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

| Layer (type)             | Output Shape          | Param #    |
|--------------------------|-----------------------|------------|
| input_6 (InputLayer)     | (None, 224, 224, 3)   | 0          |
| conv1 (Conv2D)           | (None, 112, 112, 32)  | 864        |
| conv1_bn (BatchNormaliz.)| (None, 112, 112, 32)  | 128        |
| conv1_relu (ReLU)        | (None, 112, 112, 32)  | 0          |
| ...                      | ...                   | ...        |
| conv_pw_13_relu (ReLU)   | (None, 7, 7, 1024)    | 0          |
| global_average_pooling2d | (None, 1024)          | 0          |
| dense_10 (Dense)         | (None, 128)           | 131200     |
| dropout_5 (Dropout)      | (None, 128)           | 0          |
| dense_11 (Dense)         | (None, 4)             | 516        |
|--------------------------|-----------------------|------------|
| Total params: 3,360,580  | Trainable params: 131,716 | Non-trainable params: 3,228,864 |
|--------------------------|-----------------------|------------|
