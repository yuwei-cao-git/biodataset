---
layout: default
title: Download
nav_order: 2
---

# Download the paper
[paper: A 3D INDOOR-OUTDOOR BENCHMARK DATASET FOR LoD3 BUILDING POINT CLOUD SEMANTIC SEGMENTATION](https://isprs-archives.copernicus.org/articles/XLVIII-1-W3-2023/31/2023/).

----
# Download the dataset
The BIO dataset is openly available on **Zenodo**:

[10.5281/zenodo.17400553](https://doi.org/10.5281/zenodo.17400553).

----
## File Structure Overview
```
BIO/
├─ Train/
│ ├─ Industrial_01
│ ├─ ├─ industrial_01_labelled.ply (labelled point cloud)
│ ├─ ├─ industrial_01.ply (Mesh)
│ ├─ ├─ industrial_01.obj (non-labelled 3d model)
│ ├─ ├─ industrial_01.mtl (materials)
│ ├─ ├─ industrial_01 (textures)
│ ├─ ...
├─ Val/
│ ├─ ...
├─ Test/
│ ├─ ...
```
----
# Citation

## Dataset
10.5281/zenodo.17400553

## Paper
```
@article{cao_3d_2023,
	title = {A {3D} {BUILDING} {INDOOR}-{OUTDOOR} {BENCHMARK} {FOR} {SEMANTIC} {SEGMENTATION}},
	volume = {XLVIII-1/W2-2023},
	copyright = {https://creativecommons.org/licenses/by/4.0/},
	issn = {2194-9034},
	url = {https://isprs-archives.copernicus.org/articles/XLVIII-1-W2-2023/147/2023/},
	doi = {10.5194/isprs-archives-XLVIII-1-W2-2023-147-2023},
	abstract = {Abstract. Both machine learning (ML) and deep learning (DL) algorithms require high-quality training samples as well as precise and thorough annotations in order to work effectively. The 3D building indoor-outdoor dataset (BIO dataset), which is a highly accurate, high-level of detail, and high coverage dataset for 3D building point cloud and mesh semantic segmentation, is established as a canonical benchmark dataset. It contains 100 building models, in which building structural elements are annotated into 11 semantic categories. Each building in this dataset has an average of 75,587 triangular faces, and the total area of the dataset is 481,769 square meters. Furthermore, semantic segmentation of the dataset was carried out using the Random Forest ML algorithm to verify the dataset’s accessibility. A weighted F1 score of 96.64\% was obtained with 10\% of the segments of each building randomly chosen as training data. For applications involving building geometry data, the BIO dataset can support a broad class of recently developed ML and DL methodologies.}
	language = {en},
	urldate = {2025-10-20},
	journal = {The International Archives of the Photogrammetry, Remote Sensing and Spatial Information Sciences},
	author = {Cao, Y. and Scaioni, M.},
	month = dec,
	year = {2023},
	pages = {147--153},
}
```
----

# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue, or any other method, with the owners of this repository before making a change.

# LICENSE
This dataset is distributed by an [MIT license](https://github.com/biodataset/biodataset/blob/main/LICENSE)
You may use, modify, and redistribute **with citation**.
