# Synthetic Pistachio Image Generation using GAN

![Python](https://skillicons.dev/icons?i=python) ![TensorFlow](https://skillicons.dev/icons?i=tensorflow) ![Keras](https://skillicons.dev/icons?i=keras) ![NumPy](https://skillicons.dev/icons?i=numpy) ![Matplotlib](https://skillicons.dev/icons?i=matplotlib)

**Course:** Deep Learning   
**Dataset:** Pistachio (Kirmizi) Images  
**Year:** 2025  



## About This Project
This project focuses on generating synthetic pistachio images using Generative Adversarial Networks (GAN). It includes building baseline and modified GAN models, training them on real images, and evaluating the generated images using **Fréchet Inception Distance (FID)**.


## Project Workflow

### 1. Baseline GAN Model
**Generator Architecture:**
- 3 Convolutional layers (kernel 3x3, stride 1, valid padding)  
- Number of filters: 16, 32, 64  
- Activation: ReLU (except last layer uses Tanh)  
- Output: 100x100x3 images  
- Input: Random Gaussian noise  

**Discriminator Architecture:**
- 3 Convolutional layers (kernel 3x3, stride 1, valid padding)  
- Number of filters: 16, 32, 64  
- Activation: ReLU  
- Fully connected layer with Sigmoid activation  

**Training:**
- Optimizer: Adam (Generator & Discriminator)  
- Loss: Binary Crossentropy  



### 2. Modified GAN Model
- Adjusted generator/discriminator architecture (e.g., more layers, different number of filters)  
- Applied hyperparameter tuning (learning rate, batch size, optimizer)  
- Trained model to improve synthetic image quality  



### 3. Evaluation
- Evaluated baseline and modified GAN models using **Fréchet Inception Distance (FID)**  
- Compared FID scores to assess the realism of generated images  
- Analyzed and discussed improvement from baseline to modified GAN  



## Technologies Used
- Python  
- TensorFlow & Keras  
- NumPy & pandas  
- Matplotlib & Seaborn  
- OpenCV / PIL (for image preprocessing)  
- TensorFlow-GAN or custom FID implementation  


