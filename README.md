
## Key References on Representation Learning for Earth Observation

- [Multi-Modal Self-Supervised Representation Learning for Earth Observation](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com)
- [CRA5: Extreme Compression of ERA5 for Portable Global Climate and Weather Research via an Efficient Variational Transformer](https://doi.org/10.48550/arXiv.2405.03376)
- [Remote Sensing Image Scene Classification with Self-Supervised Paradigm under Limited Labeled Samples](https://doi.org/10.48550/arXiv.2010.00882)
- [Unsupervised Severe Weather Detection Via Joint Representation Learning Over Textual and Weather Data](https://doi.org/10.48550/arXiv.2005.07243)

## Key References on Learning Representations
The paper discusses advancements in self-supervised learning (SSL) and representation learning, citing several key works:

- [A cookbook of self-supervised learning](https://doi.org/10.48550/arXiv.2304.12210) : A comprehensive review of self-supervised learning techniques, covering various paradigms beyond ImageNet-based methods.
- [An image is worth 16x16 words: Transformers for image recognition at scale](https://doi.org/10.48550/arXiv.2010.11929) : Introduces Vision Transformers (ViT), a significant shift in learning representations for visual data.
- [Masked Autoencoders Are Scalable Vision Learners](https://doi.org/10.48550/arXiv.2111.06377) : Proposes Masked Autoencoders (MAE), which have become a foundation for self-supervised learning in vision tasks.
- [DINOv2: Learning Robust Visual Features without Supervision](https://doi.org/10.48550/arXiv.2304.07193): Introduces DINOv2, a self-supervised learning approach that learns robust semantic features from images.
- [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://doi.org/10.48550/arXiv.2301.08243): Explores joint-embedding architectures for learning representations, expanding the capabilities of contrastive learning.
- [Evidence Transfer](https://doi.org/10.1109/IJCNN.2019.8852384): Evidence Transfer is a deep learning method that incrementally manipulates the latent representations of an autoencoder according to external categorical evidence.

## Key References on Semantic Representation Learning
The study highlights the importance of semantic representations and multi-modal data for generalization:

- [MultiMAE: Multi-modal Multi-task Masked Autoencoders](https://doi.org/10.48550/arXiv.2204.01678): Proposes MultiMAE, a multi-modal masked autoencoder for learning from RGB, depth, and segmentation maps.
- [4M: Massively Multimodal Masked Modeling](https://doi.org/10.48550/arXiv.2312.06647): Introduces 4M, a multi-modal masked modeling framework, where multiple input modalities are tokenized before being processed by a transformer-based autoencoder.
- [Learning Transferable Visual Models From Natural Language Supervision](https://doi.org/10.48550/arXiv.2103.00020): Introduces CLIP, a contrastive learning approach that learns from image-text pairs, influencing multi-modal representation learning.
- [Masked feature prediction for self-supervised visual pre-training](https://doi.org/10.48550/arXiv.2112.09133): Demonstrates masked feature prediction as an effective pretext task for learning high-quality representations.

## Key References on Self-Supervised Learning in EO
Since ground-level self-supervised learning techniques might be suboptimal for EO data, recent work has explored unique EO-specific self-supervised learning approaches:
### Geolocation-Based SSL:
- [Geography-Aware Self-Supervised Learning](https://doi.org/10.48550/arXiv.2011.09980) (GASSL): Introduces geography-aware self-supervised learning, leveraging EO data’s spatial-temporal structure to generate positive image pairs without artificial augmentations.
- [SatCLIP: Global, General-Purpose Location Embeddings with Satellite Imagery](https://doi.org/10.48550/arXiv.2311.17179) (SatCLIP): Trains a Sentinel-2 encoder to learn location embeddings using a contrastive learning framework.

### Time-Based SSL:
- [Seasonal Contrast: Unsupervised Pre-Training from Uncurated Remote Sensing Data](https://doi.org/10.48550/arXiv.2103.16607) (SeCo): Introduces Seasonal Contrast, a method that learns representations invariant to seasonal changes.
- [SatMAE: Pre-training Transformers for Temporal and Multi-Spectral Satellite Imagery](https://doi.org/10.48550/arXiv.2207.08051) (SatMAE): Extends MIM to image time series, enabling temporal learning from EO data.
- [Lightweight, Pre-trained Transformers for Remote Sensing Timeseries](https://doi.org/10.48550/arXiv.2304.14065) (Presto): A lightweight transformer model designed for multi-modal time series analysis, ignoring textural features.

### Modality-Based SSL:
- [Scale-MAE: A Scale-Aware Masked Autoencoder for Multiscale Geospatial Representation Learning](https://doi.org/10.48550/arXiv.2212.14532) (Scale-MAE): Proposes a scale-aware MAE that conditions on ground sampling distance (GSD).
- [SatlasPretrain: A Large-Scale Dataset for Remote Sensing Image Understanding](https://doi.org/10.48550/arXiv.2211.15660) (SatlasPretrain): Constructs a multi-task dataset for optical satellite images, utilizing diverse data sources (e.g., OSM, Lidar scans).

## Benchmarks for Earth Observation Representation Learning
- [GEO-Bench: Toward Foundation Models for Earth Monitoring](https://doi.org/10.48550/arXiv.2306.03831) GEO-Bench
Introduces GEO-Bench, a benchmark for evaluating self-supervised learning (SSL) methods on Earth Observation datasets.
Covers classification and segmentation tasks on multiple Sentinel-2-based datasets.
GEO-Bench serves as an evaluation framework for models trained on MMEarth.
-[BigEarthNet: A Large-Scale Benchmark Archive For Remote Sensing Image Understanding](https://doi.org/10.1109/IGARSS.2019.8900532). BigEarthNet: Large-Scale Datasets for Earth Observation (EO)
Land Cover and Land Use Classification Datasets

### Key References for Datasets
-  [MMEarth: Exploring Multi-Modal Pretext Tasks For Geospatial Representation Learning](https://doi.org/10.48550/arXiv.2405.02771). MMEarth: A multi-modal, global-scale pretraining dataset containing 1.2 million locations with 12 aligned modalities.

- [EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification](https://doi.org/10.48550/arXiv.1709.00029). EuroSAT
Contains ~590K Sentinel-2 images, with 43 land cover classes.
Used in GEO-Bench as BigEarth20k (a smaller, harmonized version).

- [So2Sat LCZ42: A Benchmark Dataset for Global Local Climate Zones Classification](https://doi.org/10.48550/arXiv.1912.12171) – So2Sat-LCZ42
A multi-class land cover classification dataset for Sentinel-2 imagery.
Contains 27K images, classified into 10 categories (e.g., forests, rivers, residential areas).
Used in GEO-Bench as EuroSat2k.

- [A high-resolution canopy height model of the Earth](https://doi.org/10.48550/arXiv.2204.08322). ETH-GCHM
A multi-class classification dataset for urban local climate zones (LCZ).
Contains 400K image pairs from Sentinel-1 (SAR) and Sentinel-2 (Optical).
Used in GEO-Bench as So2Sat20k.
Global Land Cover and Canopy Height Datasets

- [Dynamic World, Near real-time global 10 m land use land cover mapping](https://doi.org/10.1038/s41597-022-01307-4) – Dynamic World
A 10m-resolution Global Canopy Height Map, derived from Sentinel-2 and GEDI LiDAR data. Used in MMEarth for pixel-level vegetation height information.

- [BigEarthNet-MM: A Large Scale Multi-Modal Multi-Label Benchmark Archive for Remote Sensing Image Classification and Retrieval](https://doi.org/10.1109/MGRS.2021.3089174)
A real-time global 10m land cover dataset, generated from Google Earth Engine and Sentinel-2 imagery.
Contains 9 land cover categories.
Used in MMEarth for land cover classification.


- [SatlasPretrain: A Large-Scale Dataset for Remote Sensing Image Understanding
](https://doi.org/10.48550/arXiv.2211.15660) – SatlasPretrain
A multi-modal, multi-temporal dataset for self-supervised learning in EO.
Includes Sentinel-1 (SAR) and Sentinel-2 (Optical) imagery.


