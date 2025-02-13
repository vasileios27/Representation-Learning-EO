# State of the art


In the Earth Observation (EO) domain, Machine Learning (ML) techniques have started to be used for various tasks. However, for ML to perform efficient classification, it requires large amounts of labeled data for training and testing. In the EO domain, such datasets are rarely available and are often tailored to specific tasks.

To address these challenges in the work [[2]](https://doi.org/10.48550/arXiv.2005.07243) they have introduced an "Evidence Transfer" technique combined with a clustering algorithm, which is later used to classify extreme weather events. Similarly, self-supervised learning approaches have been explored, where representations are learned using pretext tasks and then transferred to downstream tasks. Studies such as [[3]](https://doi.org/10.48550/arXiv.2010.00882),[[1]](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com) demonstrate that even with a small labelled dataset, these methods can achieve higher accuracy compared to models pre-trained on non-EO tasks. In the paper review of Self-Supervised Learning
in Remote Sensing [[4]](https://doi.org/10.1109/MGRS.2022.3198244), it is clear that those techniques are vastly underexplored in the EO domain, compared to other fields. 

<img src="Screenshot from 2025-02-13 18-53-37.png" alt="SSL statistics" width="400">

<img src="Untitled Diagram-Page-8.drawio.png" alt="Model overview" width="600">


## Problems They Aim to Solve

 - Scarcity of Labeled Data in Earth Observation (EO)

 - The use of self-supervise learing (SSL) in EO remains underexplored [[1]](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com)

We aim to 
 - learn EO domain representations for downstream tasks with small labelled data.
 - perform better from a basline solution of outlier detection

With a carefully designed self-supervised problem, the model f gets the ability to capture high-level representations of the input data. Afterward, the model f can be further transferred to supervised downstream tasks for real-world applications.

