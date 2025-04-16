# DownSample Dataset Creator

This notebook provides a simple utility for creating **downsampled versions of facial image datasets to KDEF**.  
It generates multiple folders with the same image names, each resized to a different resolution :
- 28x28
- 56x56
- 112x112


## Features

- Batch processing of all images in KDEF-like datasets.
- Automatically organizes outputs into resolution-named folders.
- Can be used to simulate low-resolution conditions for testing face restoration models like **GFPGAN** or **CodeFormer**.

## Usage

1. Open the `DownSample_Dataset_Creator.ipynb` notebook.
2. Set the input folder path to your original dataset (e.g., KDEF).
3. Choose your target resolutions (e.g., `[28, 56, 112]`).
4. Run all cells.

Each resolution will be saved in a separate output folder

## Sample Output

Below is a sample showing the same face image downsampled at different levels:

![Downsampled Faces](https://github.com/user-attachments/assets/d818778d-abeb-4d6b-a724-84747d5d25aa)
