# Enhanced Face Resolution

This notebook applies state-of-the-art super-resolution models, such as **GFPGAN** and **CodeFormer**, to restore facial details in low-resolution or degraded images.  
The pipeline demonstrates how enhanced resolution can improve the visual quality and identity preservation of facial images under various downsampling conditions.
**All restored outputs are resized to 224×224 pixels**, making them suitable for feeding into deep learning models in subsequent processing stages(e.g VGG-16, ResNet50 etc...).


Below is an example of the same face restored from different downsampled resolutions using GFPGAN and CodeFormer:

![Enhanced GFPGAN Example](https://github.com/user-attachments/assets/e2aa10b0-4fbd-4438-8ad6-649c40b9c5a7)

![Enhanced CodeFormer Example](https://github.com/user-attachments/assets/8e4168f1-5cd3-4ad0-9918-54f29d74bb09)



## Features

- Supports restoration with both GFPGAN and CodeFormer.
- Handles extremely low-resolution inputs (e.g., 28×28).
- Accepts input images from custom datasets like KDEF.
- Displays side-by-side visual comparison of restored outputs.

## Requirements

- Python 3.8+
- OpenCV
- Matplotlib
- Pre-trained weights for GFPGAN and CodeFormer

## Usage

1. Load the notebook `Enhanced_Face_Resolution.ipynb`.
2. Specify the input image paths.
3. Choose restoration method(s): `GFPGAN`, `CodeFormer`, or both.
4. Run the notebook cells to visualize and compare the results.



> *Note: To reproduce this, make sure to downsample your images using consistent settings as in the dataset creator.*
