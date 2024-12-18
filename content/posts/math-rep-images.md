
---
title: "Mathematical Representation of Images"
date: 2024-12-04
draft: true
summary: this is summary of post 1
tag: [ "math","images"]
---


## 1. Pixel
- **What is a Pixel?**
  - A pixel is the smallest unit of an image, representing a single point in a grid.
- **Why is it important?**
  - It’s the basic building block of an image. Every image is made up of pixels, and understanding their arrangement and values is crucial for image processing.
- **How is it represented mathematically?**
  - Mathematically, a pixel in a grayscale image is represented by a scalar value (e.g., an integer from 0 to 255), while a pixel in a color image is represented by a vector of three values (Red, Green, Blue).
  - **Example:**
    - For a grayscale image: \( p_{x, y} \in \mathbb{Z} \), where \( x \) and \( y \) are the pixel coordinates, and \( p_{x,y} \) is the intensity value.
    - For an RGB image: \( p_{x, y} = (R, G, B) \), where \( R, G, B \) are the color intensity values for red, green, and blue respectively.
- **When do we use this?**
  - Every image you encounter on a digital platform is made up of pixels, whether it's a photograph, video frame, or even medical imaging.

---

## 2. Image as a Matrix
- **What is an Image Matrix?**
  - An image can be mathematically represented as a 2D or 3D matrix (depending on whether the image is grayscale or colored).
  - **Grayscale Image**: A 2D matrix \( I \) of size \( m \times n \), where each entry represents a pixel intensity.
  - **RGB Image**: A 3D matrix \( I \) of size \( m \times n \times 3 \), where the third dimension corresponds to the color channels (Red, Green, Blue).
- **Why is it important?**
  - The matrix representation allows for the application of mathematical operations, such as transformations, filtering, and feature extraction.
- **How is it represented mathematically?**
  - **Grayscale image matrix**: 
    \[
    I = \begin{pmatrix} 
    p_{1,1} & p_{1,2} & \dots & p_{1,n} \\
    p_{2,1} & p_{2,2} & \dots & p_{2,n} \\
    \vdots & \vdots & \ddots & \vdots \\
    p_{m,1} & p_{m,2} & \dots & p_{m,n} 
    \end{pmatrix}
    \]
  - **RGB image matrix**: 
    \[
    I = \begin{pmatrix}
    p_{1,1,1} & p_{1,1,2} & \dots & p_{1,1,3} \\
    p_{1,2,1} & p_{1,2,2} & \dots & p_{1,2,3} \\
    \vdots & \vdots & \ddots & \vdots \\
    p_{m,n,1} & p_{m,n,2} & \dots & p_{m,n,3}
    \end{pmatrix}
    \]
    where each entry in the matrix corresponds to a pixel's intensity for the respective color channel.
- **When do we use this?**
  - When performing operations like convolution, image transformations, or even encoding and compression.

---

## 3. Image Transformation
- **What is Image Transformation?**
  - Image transformation involves applying mathematical functions to modify the image's properties (scaling, rotation, translation, etc.).
- **Why is it important?**
  - Transformations help with tasks such as resizing, rotating, and aligning images for processing or analysis.
- **How is it represented mathematically?**
  - Image transformations are often represented by matrices. For example, a 2D affine transformation can be written as:
    \[
    \begin{bmatrix}
    x' \\
    y' \\
    1
    \end{bmatrix}
    = 
    \begin{bmatrix}
    a & b & t_x \\
    c & d & t_y \\
    0 & 0 & 1
    \end{bmatrix}
    \begin{bmatrix}
    x \\
    y \\
    1
    \end{bmatrix}
    \]
    where \( (x, y) \) are the coordinates of the original image, and \( (x', y') \) are the coordinates after the transformation. The matrix represents scaling, rotation, and translation.
- **When do we use this?**
  - Commonly used in image registration, augmented reality, and when preparing data for machine learning models.

---

## 4. Image Filtering
- **What is Image Filtering?**
  - Image filtering refers to applying a filter (kernel) to the image to modify or enhance certain features, like blurring or edge detection.
- **Why is it important?**
  - Filtering is crucial for tasks such as noise reduction, feature extraction, and sharpening images.
- **How is it represented mathematically?**
  - A filter or kernel is a small matrix that is convolved with the image matrix. For a 3x3 kernel \( K \) and a pixel \( p_{i,j} \), the filtered value \( p'_{i,j} \) is calculated as:
    \[
    p'_{i,j} = \sum_{a=-1}^{1} \sum_{b=-1}^{1} K(a,b) \cdot p_{i+a,j+b}
    \]
    where \( K(a,b) \) is the kernel value at position \( (a,b) \) and \( p_{i+a,j+b} \) are the corresponding pixel values in the image matrix.
- **When do we use this?**
  - When enhancing or extracting features in an image, especially in edge detection or smoothing.

---

## 5. Image Compression
- **What is Image Compression?**
  - Image compression is the process of reducing the size of an image while maintaining its quality as much as possible.
- **Why is it important?**
  - Compression reduces storage requirements and transmission time, which is important for handling large volumes of image data.
- **How is it represented mathematically?**
  - One common method is using Discrete Cosine Transform (DCT) for JPEG compression, where the image is transformed into the frequency domain. The DCT of a 2D image \( I(x, y) \) is computed as:
    \[
    C(u,v) = \sum_{x=0}^{M-1} \sum_{y=0}^{N-1} I(x,y) \cdot \cos \left[\frac{(2x+1)u\pi}{2M}\right] \cdot \cos \left[\frac{(2y+1)v\pi}{2N}\right]
    \]
  - The transformed coefficients are quantized, and the less significant coefficients are discarded.
- **When do we use this?**
  - In image storage, web images, and video streaming.
