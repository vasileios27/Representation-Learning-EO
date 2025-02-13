# State of the art


In the Earth Observation (EO) domain, Machine Learning (ML) techniques have started to be used for various tasks. However, for ML to perform efficient classification, it requires large amounts of labeled data for training and testing. In the EO domain, such datasets are rarely available and are often tailored to specific tasks.

To address this challenge in the work [[2]](https://doi.org/10.48550/arXiv.2005.07243) they have introduce an "Evidence Transfer" techinque combined with  clustering algorithms, which are later used to classify extreme weather event. Similarly, self-supervised learning approaches have been explored, where representations are learned using pretext tasks and then transferred to downstream tasks. Studies such as [[3]](https://doi.org/10.48550/arXiv.2010.00882),[[1]](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com) demonstrate that even with a small labeled dataset, these methods can achieve higher accuracy compared to models pre-trained on non-EO tasks.

<img src="Untitled Diagram-Page-8.drawio.png" alt="Model overview" width="600">


## Problems They Aim to Solve

 - Scarcity of Labeled Data in Earth Observation (EO)

 - The use of self-supervise learing (SSL) in EO remains underexplored [[1]](https://ieeexplore.ieee.org/document/9553741?utm_source=chatgpt.com)

We aim to 
 - learn EO domain representations for downstream tasks with small labelled data.
 - perform better from a basline solution of outlier detection

With a carefully designed self-supervised problem, the model f gets the ability to capture high-level representations of the input data. Afterward, the model f can be further transferred to supervised downstream tasks for real-world applications.

