# Image Transformation and Filtering Tool

A Python-based interactive tool for performing **geometric transformations** and **image filtering operations** using **OpenCV, NumPy, PIL, and Matplotlib**.

This project provides a **menu-driven interface** that allows users to upload an image and apply different transformations such as translation, rotation, scaling, shearing, and common filters like mean and median filters.

---

# Features

## Geometric Transformations

* **Translation** – Move the image along X and Y axes
* **Rotation** – Rotate the image by a specified angle
* **Scaling** – Resize the image using scale factors
* **Shearing** – Apply shear transformation to distort the image shape

## Image Filters

* **Upscale (Point Filter ×5)** – Enlarge image using nearest-neighbor interpolation
* **Downscale (Point Filter 1/9)** – Reduce image size using point filtering
* **Mean Filter** – Smooth the image by averaging neighboring pixels
* **Median Filter** – Remove salt-and-pepper noise

## Flexible Affine Transformation

The project also includes a **FlexibleAffine class** that allows combining multiple transformations using a **3×3 transformation matrix**.

---

# Project Structure

```
image-transform-tool/
│
├── image_transformer.py     # Main Python script
├── README.md                # Project documentation
```

---

# Technologies Used

* **Python**
* **OpenCV**
* **NumPy**
* **Matplotlib**
* **Pillow (PIL)**
* **Google Colab file upload API**

---

# Installation

Install required libraries before running the script:

```bash
pip install opencv-python numpy matplotlib pillow
```

If running locally (not on Google Colab), you may remove:

```python
from google.colab import files
```

and replace the upload section with a manual image path.

---

# How to Run

1. Open the script in **Google Colab** or your Python environment.
2. Run the program.
3. Upload an image when prompted.
4. Use the interactive menu to apply transformations.

Example menu:

```
IMAGE TRANSFORMATION MENU
==================================================
1. Geometric transformation
   1. Translation
   2. Rotation
   3. Scaling
   4. Shearing

2. Filters
   1. Upscale (Point Filter ×5)
   2. Downscale (Point Filter 1/9)
   3. Mean Filter
   4. Median Filter

0. Exit
```

---

# Example Workflow

1. Upload an image
2. Choose **Geometric Transformation**
3. Select **Rotation**
4. Enter the rotation angle
5. The transformed image will be displayed

---

# Classes in the Project

### `ImageTransformer`

Handles:

* Geometric transformations
* Image filtering
* Image display

### `FlexibleAffine`

Implements affine transformation operations using transformation matrices:

* Rotation
* Scaling
* Shearing
* Translation

---

# Learning Objectives

This project demonstrates key concepts in **Digital Image Processing**, including:

* Geometric transformations
* Affine transformations
* Spatial filtering
* Image interpolation
* Pixel manipulation

---

# Future Improvements

Possible enhancements include:

* GUI interface using **Tkinter or PyQt**
* Additional filters (Gaussian, Sobel, Laplacian)
* Histogram equalization
* Image saving functionality
* Batch processing for multiple images

---

# License

This project is for **educational purposes** and can be freely modified or used for learning.

---

# Author

Created as part of a **Digital Image Processing practice project**.
