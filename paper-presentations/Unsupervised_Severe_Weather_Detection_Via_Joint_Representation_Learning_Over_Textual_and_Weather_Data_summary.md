# Summary of: Unsupervised Severe Weather Detection Via Joint Representation Learning Over Textual and Weather Data


In the paper they try to solve the problem which is stated as  "severe cases or anomalies are often characterised by deviation from the expected data distribution. However, non-deviating data samples may also implicitly lead to severe outcomes" 

The make the statment that "We posit that incorporating external or auxiliary information, such as the outcome of an
external task or an observation, can improve the decision boundaries of an unsupervised detection
algorithm."

To establies their statment they increase the effectiveness of a clustering method to detect cases of
severe weather by learning augmented and linearly separable latent representations. They evaluate their
solution against three individual cases of severe weather, namely windstorms, floods and tornado
outbreaks. They employ the “[Evidence Transfer](https://doi.org/10.1109/IJCNN.2019.8852384)” methond.

<img src="Screenshot from 2025-02-13 12-10-40.png" alt="Evidence Transfer" width="400">

## Set-up of the experiment

- 4 severe weather cases :  (1) costly or deadly hailstorms, (2) floods, (3) tornadoes and tornado outbreaks and (4) severe windstorms. 

- Textual evidence: In summary, the textual evidence comprises a combination of structured data (dates, event types, locations, coordinates) and unstructured descriptive text (event descriptions), sourced primarily from Wikipedia and enhanced with geographic information from the GeoNames API. This information is used to augment weather data for classification tasks related to severe weather predictions.

- Each of these event types is treated as a binary classification task for predicting a specific severe
weather case. 


### Overview of the Method: Evidence Transfer for Severe Weather Detection
- Unsupervised Training a Denoising Stacked Autoencoder: 
  - weather re-analysis data.
  - A denoising stacked autoencoder with main task to reconstruct the weather data.

- Baseline Solution with Unsupervised Detection
  - latent representations from the autoencoder, used with an unsupervised clastering method to find sever events (baseline solution).

- Evidence Transfer & Latent Space Manipulation
  - Textual severe weather dataset is used as additional evidence.
  - The latent space is incrementally manipulated using this evidence.
  - The same unsupervised detection method is applied to compare effectiveness before and after evidence transfer.


