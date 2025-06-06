## 🖼️ Image Compression using PCA and K-Means Clustering
--------------------------------------------------------------
This project demonstrates how to compress and visualize images using **Principal Component Analysis (PCA)** and **K-Means clustering**.
It uses a combination of **dimensionality reduction** and **unsupervised learning** techniques to reduce the color complexity of an image while preserving the visual quality.

-----------------------------------------------------------------------

## 📌 Project Overview

- Input: RGB image 
- Dimensionality Reduction: PCA (from 3D RGB → 2D space)
- Clustering: K-Means to find  dominant colors in reduced space
- Reconstruction: Image compressed using clustered colors

-------------------------------------------------------------------------

## 🧪 Technologies Used

| Tool/Library      | Purpose                         |
|-------------------|----------------------------------|
| Python            | Programming language             |
| NumPy             | Numerical operations             |
| Matplotlib        | Visualization                    |
| PIL (Pillow)      | Image loading and manipulation   |
| scikit-learn      | PCA & KMeans implementation      |

-----------------------------------------------------------------------------

## 🚀 How It Works

 1. Load and Preprocess Image
- Load the image using PIL
- Convert RGBA to RGB if necessary
- Flatten image from shape "[h,w,s] ->[n_pixels,s]"
- Scale pixel values to range "[0,1]"

 2. Dimensionality Reduction using PCA
- Reduce RGB pixel data to 2D
- Plot a 2D scatter of image pixels
- Print variance explained by components

 3. Clustering with K-Means
- Apply KMeans on 2D PCA representation
- Choose "k" to reduce image to "k" dominant colors
- Map each pixel to its cluster center
- Reconstruct and display the compressed image

 4. Visualization
- Compare original image with compressed image
- Visualize 2D PCA scatter with original colors

----------------------------------------------------------------------------------
✍️ Author
Jefisha.C

