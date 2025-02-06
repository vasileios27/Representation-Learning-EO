
## Key References on Representation Learning for Earth Observation

- [Multi-Modal Self-Supervised Representation Learning for Earth Observation](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com)
- [CRA5: Extreme Compression of ERA5 for Portable Global Climate and Weather Research via an Efficient Variational Transformer](https://doi.org/10.48550/arXiv.2405.03376)

## Key References on Learning Representations
The paper discusses advancements in self-supervised learning (SSL) and representation learning, citing several key works:

- [A cookbook of self-supervised learning](https://doi.org/10.48550/arXiv.2304.12210) : A comprehensive review of self-supervised learning techniques, covering various paradigms beyond ImageNet-based methods.
- [An image is worth 16x16 words: Transformers for image recognition at scale](https://doi.org/10.48550/arXiv.2010.11929) : Introduces Vision Transformers (ViT), a significant shift in learning representations for visual data.
- [Masked Autoencoders Are Scalable Vision Learners](https://doi.org/10.48550/arXiv.2111.06377) : Proposes Masked Autoencoders (MAE), which have become a foundation for self-supervised learning in vision tasks.
- [DINOv2: Learning Robust Visual Features without Supervision](https://doi.org/10.48550/arXiv.2304.07193): Introduces DINOv2, a self-supervised learning approach that learns robust semantic features from images.
- [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://doi.org/10.48550/arXiv.2301.08243): Explores joint-embedding architectures for learning representations, expanding the capabilities of contrastive learning.

## Key References on Semantic Representation Learning
The study highlights the importance of semantic representations and multi-modal data for generalization:

- [MultiMAE: Multi-modal Multi-task Masked Autoencoders](https://doi.org/10.48550/arXiv.2204.01678): Proposes MultiMAE, a multi-modal masked autoencoder for learning from RGB, depth, and segmentation maps.
- [4M: Massively Multimodal Masked Modeling](https://doi.org/10.48550/arXiv.2312.06647): Introduces 4M, a multi-modal masked modeling framework, where multiple input modalities are tokenized before being processed by a transformer-based autoencoder.
- [Learning Transferable Visual Models From Natural Language Supervision](https://doi.org/10.48550/arXiv.2103.00020): Introduces CLIP, a contrastive learning approach that learns from image-text pairs, influencing multi-modal representation learning.
- [Masked feature prediction for self-supervised visual pre-training](https://doi.org/10.48550/arXiv.2112.09133): Demonstrates masked feature prediction as an effective pretext task for learning high-quality representations.

## Key References on Self-Supervised Learning in EO
Since ground-level self-supervised learning techniques might be suboptimal for EO data, recent work has explored unique EO-specific self-supervised learning approaches:
### Geolocation-Based SSL:
- Ayush et al. [3] (GASSL): Introduces geography-aware self-supervised learning, leveraging EO data’s spatial-temporal structure to generate positive image pairs without artificial augmentations.
- Klemmer et al. [25] (SatCLIP): Trains a Sentinel-2 encoder to learn location embeddings using a contrastive learning framework.

### Time-Based SSL:
- Manas et al. [29] (SeCo): Introduces Seasonal Contrast, a method that learns representations invariant to seasonal changes.
- Cong et al. [11] (SatMAE): Extends MIM to image time series, enabling temporal learning from EO data.
- Tseng et al. [46] (Presto): A lightweight transformer model designed for multi-modal time series analysis, ignoring textural features.

### Modality-Based SSL:
- Reed et al. [38] (Scale-MAE): Proposes a scale-aware MAE that conditions on ground sampling distance (GSD).
- Bastani et al. [7] (SatlasPretrain): Constructs a multi-task dataset for optical satellite images, utilizing diverse data sources (e.g., OSM, Lidar scans).

## Key References for Datasets M
-  MMEarth Dataset
Vishal Nedungadi et al.
MMEarth: A multi-modal, global-scale pretraining dataset containing 1.2 million locations with 12 aligned modalities.
Dataset: Project Page
Code: Data Collection | MP-MAE Training

### Benchmarks for Earth Observation Representation Learning
- Lacoste et al. (2023) [27] – GEO-Bench
Introduces GEO-Bench, a benchmark for evaluating self-supervised learning (SSL) methods on Earth Observation datasets.
Covers classification and segmentation tasks on multiple Sentinel-2-based datasets.
GEO-Bench serves as an evaluation framework for models trained on MMEarth.
-  Large-Scale Datasets for Earth Observation (EO)
Land Cover and Land Use Classification Datasets
Sumbul et al. (2019) [42] – BigEarthNet

### A multi-label land cover classification dataset covering 10 European countries.
- Helber et al. (2019) [23] – EuroSAT
Contains ~590K Sentinel-2 images, with 43 land cover classes.
Used in GEO-Bench as BigEarth20k (a smaller, harmonized version).

- Zhu et al. (2020) [58] – So2Sat-LCZ42
A multi-class land cover classification dataset for Sentinel-2 imagery.
Contains 27K images, classified into 10 categories (e.g., forests, rivers, residential areas).
Used in GEO-Bench as EuroSat2k.

- Lang et al. (2023) [28] – ETH-GCHM
A multi-class classification dataset for urban local climate zones (LCZ).
Contains 400K image pairs from Sentinel-1 (SAR) and Sentinel-2 (Optical).
Used in GEO-Bench as So2Sat20k.
Global Land Cover and Canopy Height Datasets

- Brown et al. (2022) [8] – Dynamic World
A 10m-resolution Global Canopy Height Map, derived from Sentinel-2 and GEDI LiDAR data.
Used in MMEarth for pixel-level vegetation height information.

- ESA World Cover (2020) [43]
A real-time global 10m land cover dataset, generated from Google Earth Engine and Sentinel-2 imagery.
Contains 9 land cover categories.
Used in MMEarth for land cover classification.

- Hersbach et al. (2020) [20] – ERA5
A 10m-resolution global land cover dataset, derived from Sentinel-1 and Sentinel-2 data.
Contains 11 land cover categories.
Used in MMEarth for land cover segmentation.
Climate and Environmental Data

- Dinerstein et al. (2017) [15] – RESOLVE Ecoregions
A global climate reanalysis dataset, providing hourly meteorological data from 1950–present.
Includes temperature, precipitation, and other atmospheric variables.
Used in MMEarth for climate-related tasks.

  
- Wang et al. (2022) [51] – SSL4EO-S12
Multi-Modal and Self-Supervised EO Datasets
Defines 846 terrestrial ecoregions across 14 biomes.
Used in MMEarth to categorize geographical regions.


A multi-modal, multi-temporal dataset for self-supervised learning in EO.
Includes Sentinel-1 (SAR) and Sentinel-2 (Optical) imagery.
- Bastani et al. (2023) [7] – SatlasPretrain


