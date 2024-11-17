# IMAGE PROCESSING USING PYTHON
Image processing refers to the manipulation and analysis of images to improve their quality or extract useful information. 
In Python, image processing can be done using several libraries, and it involves various techniques like filtering,enhancement, transformation, segmentation, and feature extraction. 
The goal is to either enhance the image for better visualization or extract meaningful data for further analysis or machine learning applications.

# DISEASE DETECTION USING GAN AND IMAGE SEGMENTATION
Using Generative Adversarial Networks (GANs) to highlight disease regions in a normal image based on a diseased image. The process involves the following steps:

- Image Preprocessing,
- Image Segmentation using Otsu's thresholding method,
- GAN Training,
- Disease Highlighting.

## REQUIREMENTS
   -Python libraries:
      -numpy
      -opencv-python (cv2)
      -tensorflow (Keras)
      -matplotlib
   -google.colab
   
## CODE EXPLAINATION
### Image Preprocessing (preprocess_image):
 -Loads images, resizes, equalizes the histogram, and normalizes pixel values.

### Otsu’s Thresholding (otsu_segmentation):
 -Applies Otsu’s method to segment the disease from the background.

### GAN Model Architecture:
 -Discriminator: A simple neural network that distinguishes between real and fake images.
 -Generator: A neural network that generates images resembling the normal image from random noise.
 
### Training Loop (train_gan):
 -The GAN is trained for a specified number of epochs. Each epoch trains the discriminator on both real and generated images, and then trains the generator to fool the discriminator.

### Disease Visualization (highlight_disease):
 -The disease mask is applied to the normal image, and both are blended for better visualization.

