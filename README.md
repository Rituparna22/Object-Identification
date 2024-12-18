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

