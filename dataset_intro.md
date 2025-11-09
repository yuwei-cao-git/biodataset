---
layout: default
title: Dataset Introduction
nav_order: 2
---

# Dataset Details

## Building Types (100 Total)

| Category | Count | Notes |
|---------|-------|-------|
| Residential | 25 | Houses, apartments, villas |
| Commercial | 25 | Offices, retail, shops |
| Industrial | 25 | Warehouses, plants |
| Institutional | 25 | Schools, hospitals, public service buildings |

---

## Semantic Classes (11)

The semantic labels follow **CityGML 3.0** + **IFC** standards:

| ID | Class | Description |
|---:|------|-------------|
| 0 | Wall | Vertical load-bearing / partition surfaces |
| 1 | Roof | Exterior top surfaces |
| 2 | Window | Transparent/opening structure |
| 3 | Door | Entry opening structures |
| 4 | Balcony | Cantilevered extensions |
| 5 | Floor | Horizontal interior surfaces |
| 6 | Stairs | Staircases |
| 7 | Column | Vertical structural elements |
| 8 | Ceiling | Indoor upper surfaces |
| 9 | Beam | Horizontal structural elements |
|10 | Slab | Structural floors / plates |

---

## Point Cloud Properties

| Property | Value |
|---------|-------|
| Sampling | Uniform surface sampling |
| Avg. points / building | ~3,500,000 |
| Attributes | XYZ, RGB, Semantic Label |

---

## Train / Val / Test Split

| Split | Building Count |
|------|----------------|
| Train | 70 |
| Validation | 15 |
| Test | 15 |

## 🧠 Benchmark Results

We trained and evaluated four **deep learning** architectures and one **machine learning baseline**:

- **PointNet** (Qi et al., 2017a)  
- **PointNet++** (Qi et al., 2017b)  
- **DGCNN** (Wang et al., 2019)  
- **RandLA-Net** (Hu et al., 2020)

### **Deep Learning Results**

| Method     | OA (↑) | mIoU (↑) |
|-----------|-------:|---------:|
| PointNet  | 0.656  | 0.188    |
| PointNet++| 0.662  | 0.198    |
| **DGCNN** | **0.835** | 0.294 |
| **RandLA-Net** | 0.518 | **0.336** |

### **Per-Class IoU Breakdown**

| Class | PN | PN++ | DGCNN | RandLA |
|------|---:|----:|------:|-------:|
| Wall      | 0.430 | 0.586 | 0.578 | **0.584** |
| Roof      | **0.735** | 0.275 | **0.787** | 0.229 |
| Window    | 0.000 | 0.000 | 0.025 | **0.167** |
| Door      | 0.000 | 0.000 | 0.000 | **0.216** |
| Balcony   | 0.002 | 0.000 | 0.003 | **0.505** |
| Floor     | 0.712 | **0.974** | 0.915 | 0.622 |
| Stairs    | 0.000 | 0.040 | 0.012 | **0.053** |
| Column    | 0.000 | 0.000 | **0.407** | 0.097 |
| Ceiling   | 0.188 | 0.003 | 0.000 | **0.355** |
| Beam      | 0.000 | 0.000 | 0.000 | **0.572** |
| Slab      | 0.000 | 0.300 | **0.509** | **0.584** |

### **Random Forest Baseline**

| Training Data Used | Weighted F1 (↑) | OA (↑) |
|-------------------|----------------:|------:|
| 1% per building   | 0.860 | 0.878 |
| 10% per building  | **0.966** | **0.969** |
