# Project Description


This project focuses on enhancing low-resolution and noisy CT images using Super-Resolution Generative Adversarial Networks (SRGANs). SRGANs are deep learning models designed to generate high-resolution images from low-resolution inputs, providing sharper and more detailed results. The goal is to improve the quality of medical imaging for better diagnosis and analysis.


# Features


Super-Resolution Enhancement: The SRGAN model is trained to upscale low-resolution CT images to higher resolutions, improving image quality.

Noise Reduction: In addition to upscaling, the model also works to reduce noise in the images, resulting in cleaner and more accurate representations.

Deep Learning Architecture: The SRGAN architecture includes components like generator and discriminator networks, along with additional features like residual blocks and perceptual loss for improved performance.

Training and Evaluation: The project includes training the SRGAN model on a dataset of low-resolution CT scans and evaluating its performance on test data. Metrics such as loss functions and image quality are used for evaluation.



# Code Structure and Usage

1. Data Preparation
Data Download: The code downloads a dataset of chest CT scan images from a specified URL and prepares it for training and testing.

Image Preprocessing: Images are resized and converted to grayscale to match the input requirements of the SRGAN model.


2. Low-Resolution Image Generation
Adding Noise: Random noise is added to the original images to simulate low-resolution and noisy inputs for the SRGAN model.

Image Resizing: The noisy images are resized to lower resolutions to serve as input for the SRGAN.

3. Model Building
Generator Network: The SRGAN's generator network is defined, which takes low-resolution images as input and outputs high-resolution versions.

Discriminator Network: A discriminator network is also defined to distinguish between generated high-resolution images and real high-resolution images.

Loss Functions: Binary cross-entropy loss and mean squared error loss are used to train the generator and discriminator networks.


4. Training
Training Loop: The generator and discriminator networks are trained iteratively on batches of low-resolution and high-resolution images.

Monitoring Loss: Loss values for both the generator and discriminator are monitored during training to assess model performance.


5. Testing and Evaluation
Generating High-Resolution Images: The trained generator is used to generate high-resolution images from test low-resolution images.

Visualizing Results: Generated high-resolution images are compared with ground truth high-resolution images to evaluate the model's performance.

