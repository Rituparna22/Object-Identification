# Object Detection using RCNN
This ia a short object detection project based on an Aquarium dataset. 
The code explores Region based Convolutional Neural Networks(RCNN). 
What is RCNN?
RCNN is a deep learning architecture that helps in Object Detection by combining CNN and region based approaches.
![RCNN](https://github.com/user-attachments/assets/8e954c34-ecd6-40c9-8ccc-7a0f58c44916)
Let's try and understand the image shown above.
First we take an input image. This input imaage goes through a region extraction process which is termed as "region proposal" or "Region Candidates".
Then we have a large convolutional neural network that extracts different feature from each region.
The last part of the process is the computation of the CNNs and the extraction of the features specific to the image. 

In our case, the images are all aquarium/sealife based. Let us have a quick and deeper look into the project.
1. The dataset used is from  https://www.kaggle.com/datasets/sharansmenon/aquarium-dataset 
2. We then format the data in the COCO format. This helps us to catagorise and organise our datasets.
3. In order to augument our data, we use albumentation, a pytorch library. (You can find out more details in https://albumentations.ai/docs/examples/pytorch_classification/)
4. After we load the data, we then check if the bounding is accurate or not by viewing a sample from the dataset. 
![image](https://github.com/user-attachments/assets/73bcc5f6-5162-4275-96b4-48d8a95c8ce3)


5. We then start with our RCNN. We choose the `MobileNetV3-Large` model. This particular model was trained on 90 classes, but since we have 7 classes, we will train it accordingly.
6. We then go on to the choice of the optimiser, and then we go on to define the function that trains the model.
7. Then we start ti experiment with the model. Here I have experimented with 20 epochs, you may take lesser or more epochs and check for different conditions (Well the world is your canvas isn't it?!) .
8. Finally we check whether or not our model has trained and is giving us the desired result.
![image](https://github.com/user-attachments/assets/39eb8623-672a-4f8c-adf0-86a042b8b0e7)

So well what do you think??? Did it work?
