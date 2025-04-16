# Enhanced Face Resolution

This notebook applies state-of-the-art super-resolution models, such as **GFPGAN** and **CodeFormer**, to restore facial details in low-resolution or degraded images.  
The pipeline demonstrates how enhanced resolution can improve the visual quality and identity preservation of facial images under various downsampling conditions.
**All restored outputs are upsampled to 224×224 pixels**, making them suitable for feeding into deep learning models in subsequent processing stages(e.g VGG-16, ResNet50 etc...).


Below is an example of different downsampled resolutions:

![downsample_comparison (1)](https://github.com/user-attachments/assets/4d0ca179-4814-46dc-9f99-1b593f9199bc)

Here is an example of the same face restored from different downsampled resolutions using GFPGAN and CodeFormer:

### GFPGAN 
![Enhanced GFPGAN Example](https://github.com/user-attachments/assets/e2aa10b0-4fbd-4438-8ad6-649c40b9c5a7)
### CodeFormer
![Enhanced CodeFormer Example](https://github.com/user-attachments/assets/8e4168f1-5cd3-4ad0-9918-54f29d74bb09)

> ⚙️ **Note**: For the CodeFormer results, we fixed the controllable parameter `w` to **0.8**, balancing visual quality and identity fidelity.  
> This choice is based on the assumption that our primary goal is **not to reconstruct the exact facial identity**, but rather to **recover the facial expression**.  
> Therefore, perfect identity preservation is less critical than maintaining expression-related features.



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
