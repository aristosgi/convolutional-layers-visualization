# Convolutional Layers Visualization

## Introduction

This repository explores the application of convolutional filters and pooling operations on images using TensorFlow. It aims to provide a practical demonstration of how these fundamental components of convolutional neural networks (CNNs) work to extract features from images.

## Features

- **Image Preprocessing**: The project includes functions to load images, resize them to a standard size, and normalize pixel values for compatibility with TensorFlow.
  
- **Convolutional Filters**: It defines and applies two essential convolutional filters: vertical and horizontal. These filters highlight vertical and horizontal edges respectively, crucial for image feature extraction.
  
- **Max Pooling**: After convolution, max pooling is applied to downsample feature maps. This step retains the most significant features while reducing computational load and enhancing computational efficiency.

**Average Pooling**: After convolution, average pooling is applied to downsample feature maps. This process computes the average value of each non-overlapping 2x2 patch of the feature map. Unlike max pooling, which retains the maximum activation, average pooling retains the average activation across the patch. This technique helps to reduce the spatial dimensions of the feature map, capturing the general presence of features rather than their precise locations. Average pooling can be beneficial in scenarios where preserving more spatial information or smoothing out noise in the feature maps is desirable.

  
- **Visualization**: The results of each step (original image, convolved images, and pooled images) are visualized using Matplotlib. This visualization aids in understanding how convolution and pooling alter the image representations.

## Installation

To run the project, ensure you have Python 3.x installed along with the following libraries:

- TensorFlow
- NumPy
- Matplotlib
- OpenCV (cv2)

You can install these dependencies using pip:

~~~
pip install tensorflow numpy matplotlib opencv-python
~~~


## Usage

1. **Clone the Repository**: Clone this repository to your local machine.

~~~
git clone https://github.com/aristosgi/convolutional-layers-visualization.git
cd convolutional-layers-visualization
~~~


2. **Run the Example**: Modify the `main` function in `main.py` to specify your image paths or use the provided examples. Then, run the script to see convolutional and pooling operations applied to your images.

```python
from main import main

# Example of a cat
print('Example of a cat')
main('photos/images.jpeg')

# Example of a block of flats
print('Example of a block of flats')
main('photos/block.jpeg')

