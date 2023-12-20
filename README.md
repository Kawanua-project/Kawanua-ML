# Kawanua Machine Learning Documentation

## Description
Our model aims to classify specific endangered species found in Indonesia:

1. *Rafflesia arnoldii* (Corpse Lily): Known for its enormous flowers, it's a rare and endangered species, considered the largest individual flower on Earth.

2. *Anaphalis javanica* (Javanese Edelweiss): A rare mountain flower symbolizing purity and endurance, found in high elevations in Indonesia.

3. *Pongo pygmaeus* (Orangutan): An iconic species of great ape native to Indonesia, known for its intelligence and arboreal lifestyle.

4. *Elephas maximus* (Asian Elephant): An endangered species essential to Indonesian ecosystems, revered for its intelligence and social behavior.

## Method
To accomplish this classification task, we harness the power of Convolutional Neural Networks (CNNs), a cutting-edge technology in image recognition and classification.

## Tools and Libraries
1. **Python:**
   - TensorFlow and Keras
   - Matplotlib
   - NumPy
   - Pandas
   - ImageDataGenerator (for data handling and preprocessing)
   - splitfolders (for data handling and preprocessing)
   - os library (for file operations)

2. **Pre-trained Model:**
   - MobileNet

3. **Google Colab**

## Datasets
Our final dataset is a collection from various sources, primarily obtained from Kaggle and through Google search scraping. Here is the link to our final datasets: [Kawanua Datasets](https://github.com/Kawanua-project/Kawanua-ML/Datasets).

## Model Acrhitecture
We integrated MobileNet as the foundational model and extended it by appending additional layers to tailor it to our specific requirements.

- Total params: 3,360,580
- Training Loss: 0.0520
- Training Accuracy: 99.37%
- Validation Loss: 0.0150
- Validation Accuracy: 99.50%

## Model Deployment
For deploying the model, we employ Flask API, a web framework in Python, which enables us to serve the machine learning model as an API.

