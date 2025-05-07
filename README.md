# Neural Style Transfer

This project implements neural style transfer using a pre-trained VGG19 model to transform the content of one image into the style of another image. The neural network optimizes an image to match the content of the original content image and the style of the style image, using a loss function that combines both content and style losses.

## Overview

Neural Style Transfer (NST) is a technique used to blend two images together: a content image and a style image. The resulting image preserves the content of the first image but takes on the artistic style of the second image. This is achieved by training a deep learning model (typically a Convolutional Neural Network, CNN) to minimize the difference between content and style representations in each image.

In this project:

* We use a **pre-trained VGG19 model** to extract the features of the content and style images.
* We optimize an initial image (starting with the content image) to match both the content and style representations.
* We perform the optimization using gradient descent, adjusting the generated image iteratively to reduce the loss.

## Dependencies

This project requires the following Python libraries:

* `torch`: For building and training the neural network.
* `torchvision`: For using the pre-trained VGG19 model and image transformations.
* `numpy`: For array manipulation and matrix operations.
* `PIL` (Python Imaging Library): For image processing.
* `matplotlib`: For visualizing the results.
* `requests`: For fetching remote images.

## Usage

1. **Prepare the content and style images**:

   * Ensure the content and style images are accessible via URL or local file path.

2. **Perform style transfer**:

   * The style transfer process will combine the content of the content image and the style of the style image into a new stylized image.

   * You can configure the number of optimization steps, save intervals, and model settings as per your preference.

3. **Visualize Results**:

   * After the style transfer process completes, you can view the content, style, and generated images. These will demonstrate how the content of one image is blended with the style of the other.

## Results

The output will include three images:

* **Content Image**: The original content image.
* **Style Image**: The original style image.
* **Stylized Image**: The generated image that combines the content of the content image and the style of the style image.

You can compare how different content and style images affect the final result by running multiple experiments.

### Example:

After running the style transfer process, you might see results similar to:

* **Content Image**: A portrait or photograph that will provide the content for the stylization.
* **Style Image**: A famous artwork or artistic style to transfer to the content image.
* **Stylized Image**: The final result, showing the content image painted in the style of the chosen artwork.

![image](https://github.com/user-attachments/assets/1d3075a9-5a3d-45c7-9f8c-637b9679b7a2)

