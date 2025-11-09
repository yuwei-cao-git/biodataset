---
layout: home
title: BIODataset
---
# BIO Dataset: 3D Indoor–Outdoor Building Semantic Segmentation Benchmark

## Introduction

To perform effectively, machine learning (ML) and deep learning (DL) algorithms require high-quality training samples and accurate and detailed annotations. We describe a semi-automatic framework for creating a dataset and establish a canonical benchmark dataset, the 3D building indoor outdoor dataset (BIO dataset), which is a highly accurate, high level of detail, and high coverage dataset for 3D building point cloud and mesh semantic segmentation. According to statistics, the total area of this dataset is 481,769 square metres, with an average of 75,587 triangular faces per building, and it contains 11 building structure semantic categories.

This dataset enables the training and evaluation of **deep learning** and **machine learning** models for built-environment understanding in applications such as:
- Indoor navigation
- Digital twins
- Facility management (BIM/GIS integration)
- Urban modelling and simulation
- Energy efficiency and structural analysis

----
## 🔍 Key Features

| Feature | Description |
|--------|-------------|
| Total Buildings | **100** (Residential, Commercial, Industrial, Institutional) |
| Representation | Polygonal Mesh + Uniform Dense Point Cloud |
| Point Count | ~3.5 million points per building |
| Semantic Classes | 11 structural classes (CityGML + IFC based) |
| LoD Level | LoD3 (with optional abstraction to LoD2 / LoD1) |
| File Formats | `.ply`, `.obj`, `.mtl`, `.stl` |
| Splits Provided | Train/Validation/Test |

----

## Some examples of our dataset

![Alt text](imgs/BIO_dataset_overview.jpeg "Some examples of the BIO dataset")

----

## Statistics of BIO dataset
![Alt text](imgs/total_class_dist.svg "Categories statistic of the BIO dataset")


## 📄 Citation

If you use BIO dataset in your research, please cite:
Cao, Y. and Scaioni, M.: A 3D INDOOR-OUTDOOR BENCHMARK DATASET FOR LoD3 BUILDING POINT CLOUD SEMANTIC SEGMENTATION, Int. Arch. Photogramm. Remote Sens. Spatial Inf. Sci., XLVIII-1/W3-2023, 31–37, https://doi.org/10.5194/isprs-archives-XLVIII-1-W3-2023-31-2023, 2023.
