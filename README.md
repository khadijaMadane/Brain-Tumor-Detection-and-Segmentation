# Brain Tumor Detection & Segmentation 

This project utilizes deep learning techniques for brain tumor segmentation in MRI images. Using a U-Net model implemented in TensorFlow, the goal is to accurately detect and segment brain tumors in medical images.

## Project Overview

This project is aimed at automating the segmentation of brain tumors in MRI scans. The U-Net model, a convolutional neural network designed for image segmentation, is used for this task. The model is trained on a dataset of MRI images with labeled tumor regions, and the goal is to predict tumor regions in unseen MRI images.

## Technologies Used

- **TensorFlow**: For deep learning model development.
- **Keras**: High-level neural networks API, running on top of TensorFlow.
- **NumPy & Pandas**: For data handling and manipulation.
- **Matplotlib**: For visualizations and plotting.
- **OpenCV**: For image processing tasks.
- **scikit-learn**: For model evaluation and metrics.
- **tqdm**: For progress bar during training.

## Dataset

This project uses MRI images of the brain, where each image is labeled with a binary mask indicating the tumor region. The dataset used is publicly available and can be found on various open datasets platforms.

## Model

The core of the project is the U-Net architecture, which is particularly well-suited for biomedical image segmentation tasks. The U-Net model consists of a contracting path to capture context and a symmetric expanding path that enables precise localization.

### U-Net Architecture
- **Encoder**: Multiple convolutional layers followed by max-pooling operations.
- **Bottleneck**: The deepest part of the network, where the features are most compressed.
- **Decoder**: Upsampling and concatenation with encoder features to make precise pixel-wise predictions.

## How to Use



