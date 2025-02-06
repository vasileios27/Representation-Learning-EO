
## Key References on Representation Learning for Earth Observation

- [Multi-Modal Self-Supervised Representation Learning for Earth Observation](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com)
- [CRA5: Extreme Compression of ERA5 for Portable Global Climate and Weather Research via an Efficient Variational Transformer](https://doi.org/10.48550/arXiv.2405.03376)

## Key References on Learning Representations
The paper discusses advancements in self-supervised learning (SSL) and representation learning, citing several key works:

- Balestriero et al. [5]: A comprehensive review of self-supervised learning techniques, covering various paradigms beyond ImageNet-based methods.
Dosovitskiy et al. [16]: Introduces Vision Transformers (ViT), a significant shift in learning representations for visual data.
- He et al. [22]: Proposes Masked Autoencoders (MAE), which have become a foundation for self-supervised learning in vision tasks.
- Oquab et al. [34]: Introduces DINOv2, a self-supervised learning approach that learns robust semantic features from images.
- Assran et al. [2]: Explores joint-embedding architectures for learning representations, expanding the capabilities of contrastive learning.

## Key References on Semantic Representation Learning
The study highlights the importance of semantic representations and multi-modal data for generalization:

- Bachmann et al. [4]: Proposes MultiMAE, a multi-modal masked autoencoder for learning from RGB, depth, and segmentation maps.
- Mizrahi et al. [31]: Introduces 4M, a multi-modal masked modeling framework, where multiple input modalities are tokenized before being processed by a transformer-based autoencoder.
- Radford et al. [37]: Introduces CLIP, a contrastive learning approach that learns from image-text pairs, influencing multi-modal representation learning.
- Wei et al. [52]: Demonstrates masked feature prediction as an effective pretext task for learning high-quality representations.

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

## Key Reference on GEO-Bench
The GEO-Bench dataset is a benchmark for evaluating Earth Observation (EO) models:

- Lacoste et al. [27]: Introduces GEO-Bench, a standardized benchmark for Earth Observation models, designed to evaluate self-supervised learning methods across different EO tasks, including classification and segmentation.
