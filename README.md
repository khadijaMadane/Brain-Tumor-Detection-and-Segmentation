# Brain Tumor Detection & Segmentation 

This project utilizes deep learning techniques for brain tumor segmentation in MRI images. Using a U-Net model implemented in TensorFlow, the goal is to accurately detect and segment brain tumors in medical images.

## Overview

This project focuses on the detection and segmentation of brain tumors from MRI scans using state-of-the-art deep learning architectures. It leverages various semantic segmentation models to provide accurate and efficient tumor detection.

The primary goal is to compare the performance of different models for medical image segmentation tasks and evaluate their efficiency in terms of metrics like Loss, Dice Coefficient, IoU, Recall, and Precision.

## Dataset

The **LGG Segmentation Dataset** contains brain MRI images and manual FLAIR (Fluid-Attenuated Inversion Recovery) abnormality segmentation masks. The data comes from **The Cancer Imaging Archive (TCIA)** and includes images from 110 patients with lower-grade gliomas, part of **The Cancer Genome Atlas (TCGA)** collection.

- **Content**: MRI images with tumor segmentation masks for FLAIR abnormalities.
- **Genomic Data**: Includes genomic subtypes and patient data (available in `data.csv`).
- **Source**: [LGG MRI Segmentation Dataset on Kaggle](https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation)

For further details, see the following publications:
- "Association of genomic subtypes of lower-grade gliomas with shape features automatically extracted by a deep learning algorithm" (Computers in Biology and Medicine, 2019).
- "Radiogenomics of lower-grade glioma: algorithmically-assessed tumor shape is associated with tumor genomic subtypes" (Journal of Neuro-Oncology, 2017).


## Models Used
- **DeepLabV3+**: Advanced semantic segmentation architecture with Atrous Spatial Pyramid Pooling (ASPP).
- **UNet**: Classic biomedical segmentation model with a U-shaped encoder-decoder structure.
- **Attention-UNet**: Improved UNet with attention mechanisms for focusing on relevant regions.
- **V-Net**: 3D convolution-based architecture designed for volumetric medical images.
- **UNETR**: Combines transformers with UNet for long-range feature learning.
- **SegNet**: Lightweight encoder-decoder model for efficient segmentation.

## Evaluation Metrics
The models are evaluated based on the following:
- **Loss**: Measures model optimization.
- **Dice Coefficient**: Measures overlap between predicted and ground truth.
- **IoU (Intersection over Union)**: Quantifies prediction accuracy.
- **Recall**: Captures sensitivity to tumor detection.
- **Precision**: Indicates the quality of tumor segmentation.

## Results
| Model           | Loss   | Dice Coefficient | IoU    | Recall | Precision |
|------------------|--------|------------------|--------|--------|-----------|
| **DeepLabV3+**   | 0.1079 | 0.8920           | 0.8060 | 0.8916 | 0.9124    |
| **UNet**         | 0.1268 | 0.8731           | 0.7766 | 0.8849 | 0.9084    |
| **Attention-UNet** | 0.1050 | 0.8949         | 0.8107 | 0.9045 | 0.8939    |
| **V-Net**        | 0.1336 | 0.8663           | 0.7681 | 0.8606 | 0.8921    |
| **UNETR**        | 0.2302 | 0.7698           | 0.6298 | 0.6931 | 0.8794    |
| **SegNet**       | 0.1401 | 0.8598           | 0.7551 | 0.8877 | 0.8590    |


 ## Model Evaluation
The model performance was evaluated on a test dataset using various metrics commonly used for image segmentation tasks. The evaluation metrics, including loss, Dice coefficient, IoU (Intersection over Union), recall, and precision, were computed to assess the effectiveness of the model in segmenting the tumor regions.

The following screenshot shows the evaluation results for the model on the test dataset, including key metrics such as the Dice coefficient, IoU, Recall, Precision, and Test Loss:

<img src="Images/res5.png" width="1000"/>

## Results
Sample visualizations of predictions vs true masks are displayed after testing, showcasing the model's performance on various MRI images.
<img src="Images/res1.png" width="500"/>
<img src="Images/res2.png" width="500"/>
<img src="Images/res3.png" width="500"/>
<img src="Images/res4.png" width="500"/>

## Contributing

We welcome contributions! Please feel free to submit issues or pull requests. If you have any questions or need support, feel free to reach out. We welcome any contributions that enhance the project's scope and impact.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



