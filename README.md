# Classifying Images: American Sign Language

## Dataset <a href="https://www.kaggle.com/datasets/grassknoted/asl-alphabet" ><img src="https://img.shields.io/badge/dataset-kaggle-green" /></a>



For this project, I  have pulled data from a Kaggle Dataset containing 87,000 images of size 200x200 pixels. These images are already categorized into 29 classes, with 26 classes representing English letters, and 3 classes representing images that do not contain American Sign Language symbols, such as “space”, “delete”, and images with no hand present.

In order to add noise to the dataset and to limit a model's tendency to overfit, I initalized a data pipeline using the Python Augmentor Pipeline. Within this pipeline are two operations applied with 30% probability: zoom and random brightness. I did not apply operations like reflections or rotations, as these operations could potentially impact the symbol being represented within the image

## 100,000 Sampled Images using Adam Optimizer and .005 Learning Rate (10 epochs)

<img src="https://user-images.githubusercontent.com/91431295/206310841-90671c2a-58ba-411f-9c8e-a2052988d717.png" width="500" height="500">
<img src="https://user-images.githubusercontent.com/91431295/206311194-2887f017-efdc-4887-8e35-fb83a0fbe5a0.png" width="500" height="300">    


## 100,000 Sampled Images using Adam Optimizer and .005 Learning Rate with Dropout (3 epochs)     

<img src="https://user-images.githubusercontent.com/91431295/206311476-e8bea001-833b-4b9e-96b4-13de4a709c88.png" width="500" height="500">
<img src="https://user-images.githubusercontent.com/91431295/206311489-a97c61f8-04a9-40cb-9c54-80514ea1ab82.png" width="500" height="300">  
                                    
## 15,000 Sampled Images using SGD Optimizer and .005 Learning Rate (10 epochs)
<img src="https://user-images.githubusercontent.com/91431295/205479514-d19c521d-0081-428b-a254-df3201ab4951.png" width="500" height="500">

<img src="https://user-images.githubusercontent.com/91431295/205479520-f46097f0-f015-42e7-ba63-f04c74fd5de7.png" width="500" height="300">


## 100,000 Sampled Images using SGD Optimizer and .005 Learning Rate (10 epochs)
<img src="https://user-images.githubusercontent.com/91431295/205480237-cd91f6bb-a422-4e5c-94dc-0ac2c15e1aec.png" width="500" height="300">

