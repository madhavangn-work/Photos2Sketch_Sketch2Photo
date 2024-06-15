
## Description

This project leverages Convolutional Autoencoder and U-Net architectures for the tasks of converting facial photos to sketches and vice versa. The dataset used is the CUHK dataset, which includes cropped photos and corresponding sketches.

### Models

1. **Convolutional Autoencoder (ConvAE)**
   - An unsupervised learning algorithm that encodes images into a lower-dimensional space and decodes them back to their original dimension.
   - Applied to both Photo2Sketch and Sketch2Photo tasks.

2. **U-Net**
   - A convolutional neural network architecture designed for image segmentation, adapted for image-to-image translation tasks.
   - Applied to both Photo2Sketch and Sketch2Photo tasks.

## Data

- **CUHK_training_cropped_photos/**: Contains the cropped photos used for training the models.
- **CUHK_training_cropped_sketches/**: Contains the corresponding cropped sketches used for training the models.

## Notebooks

### P2S (Photo2Sketch)

- **CUHK_P2S_ConvAE.ipynb**: Implements the Convolutional Autoencoder model for Photo2Sketch conversion using the CUHK dataset.
- **UNet_P2S.ipynb**: Implements the U-Net model for Photo2Sketch conversion.

### S2P (Sketch2Photo)

- **CUHK_S2P_ConvAE.ipynb**: Implements the Convolutional Autoencoder model for Sketch2Photo conversion using the CUHK dataset.
- **UNet_S2P.ipynb**: Implements the U-Net model for Sketch2Photo conversion.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- Jupyter Notebook
- TensorFlow
- Other dependencies listed in the notebooks (e.g., numpy, matplotlib)

### Running the Project

1. **Prepare the Data**:
   - Place the training images in `data/raw/CUHK_training_cropped_photos` and `data/raw/CUHK_training_cropped_sketches`.

2. **Run the Notebooks**:
   - For Photo2Sketch conversion, run the notebooks in the `src/P2S` folder:
     - `CUHK_P2S_ConvAE.ipynb`
     - `UNet_P2S.ipynb`
   - For Sketch2Photo conversion, run the notebooks in the `src/S2P` folder:
     - `CUHK_S2P_ConvAE.ipynb`
     - `UNet_S2P.ipynb`

3. **Evaluate and Compare Models**:
   - Compare the results of the Convolutional Autoencoder and U-Net models for both tasks to determine which model performs better.
