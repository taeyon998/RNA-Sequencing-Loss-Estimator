# RNA-Sequencing-Loss-Estimator

### Estimate how much gene information has been lost in a single cell RNA sequenced dataset
<br>

## Background
RNA single-cell sequencing is a transformative technology that significantly enhances our understanding of cellular functions and genetic diversity on a microscopic level. However, during the sequencing process, a portion of genetic information is inevitably lost.

To understand why genetic information is lost, it's essential to comprehend the role of Unique Molecular Identifiers (UMIs). UMIs are critical for labeling individual RNA molecules, enabling the precise tracking and quantification of genetic expression in cells. Despite this, sequencing machines face limitations, resulting in not all UMIs being captured. To mitigate this, UMIs are amplified extensively, enhancing the likelihood of detection. Nevertheless, this amplification leads to disparities where some UMIs have multiple detected copies, while others are not detected at all. This discrepancy is evident in the following graph, where 0-counts indicate UMIs that went unsequenced:
<br>
<br>
<img width="50%" src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/UMI%20counts.png">
<br>
<br>
Addressing these 0-counts is crucial. A high proportion of 0-counts suggests significant loss of original genetic information, indicating a need for deeper sequencing to achieve comprehensive data coverage. Conversely, a low proportion of 0-counts implies that the sequencing has effectively captured the majority of genetic information. My objective is to employ statistical distributions to accurately estimate these unaccounted 0-counts, thereby refining our understanding of "RNA sequencing loss."

The importance of resolving this issue cannot be overstated. By accurately estimating 0-counts, my tool aims to significantly enhance the reliability and completeness of RNA single-cell sequencing data, benefiting researchers and advancing the field.
<br>
<br>
<br>

## Workflow
<img src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/workflow.png">
<br>
<br>
<br>

## Model Estimate Results

|        |        |
| ------ | ------ |
|    <img src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/GetImage.png">     |    <img src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/GetImage (1).png">     |
|    <div align=center> `5k pbmc cells (10x genomics v3 NEXTGEM)` </div>    |    <div align=center> `5k neuron cells (10x genomics v3 NEXTGEM)` </div>    |
|    <img src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/GetImage (2).png">    |    <img src="https://github.com/taeyon998/RNA-Sequencing-Loss-Estimator/blob/main/images/GetImage (3).png">    |
|    <div align=center> `5k pbmc cells (10x genomics v3)` </div>    |    <div align=center> `9k neuron cells (10x genomics v3)` </div>    |
