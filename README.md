# Face-Recognition-by-TRANSFER-LEARNING
### Transfer Learning in Deep Neural Networks - The easiest way to describe transfer learning is the use of previously acquired knowledge and skills in new learning or problem-solving situations.     
--> In transfer learning, we reuse the weights of one or more layers from a pre-trained neural network model in our new model and either keeping the weights fixed, fine tuning them, or adapting the weights entirely when training the model.     
--> This is the same way in which we humans learn something. Humans have an inherent ability to transfer knowledge across tasks. What we acquire as knowledge while learning about one task, we utilize in the same way to solve related tasks.     
Example- Know how to ride a motorbike ⮫ Learn how to ride a car       
### I've used the concept of transfer learning in deep neural networks to train face images and do Face recognition. The pre-trained model that I've used is VGG16.   

## I've divided this project into 2 parts-    
## 1) **For dataset creation**- 
I've used **Open-CV library** and **Haar Cascade classifiers** for detecting the face.     
--> The dataset has been divided into two sets- train set and test set.      
For **train set**, the code captures 1000 images of the person's face. For the **test set**, the code captures 500 images of the person's face.   
## About Open-CV -    
OpenCV is a huge open-source library for the computer vision, machine learning, and image processing. By using it, one can process images and videos to identify objects, faces etc. I have used this library and its cv2 function to click images of face of the person from the Webcam of the Laptop/PC.
## About Haar Cascade-
Haar Cascade is a machine learning object detection algorithm used to identify objects in an image or video. The Haar Cascade is trained by superimposing the positive image over a set of negative images. The training is generally done on a server and on various stages. I have used Haar Cascade Frontal face pre trained model in this project to detect the person's face.

## 2) **For training of VGG16 and testing the model**- 
### For Training-
Firstly I've imported the VGG16 model and then its weights from ImageNet. In my new model, I have freezed all the intermediate layers of VGG except the Input and Output layer. I've trained the output layer according to my requirement.       
## About VGG16 - 
VGG16 is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford. The model achieves 92.7% top-5 test accuracy in ImageNet, which is a dataset of over 14 million images belonging to 1000 classes. It was one of the famous model submitted to ILSVRC-2014. It makes the improvement over AlexNet by replacing large kernel-sized filters (11 and 5 in the first and second convolutional layer, respectively) with multiple 3×3 kernel-sized filters one after another.

--> With the help of transfer learning, I'm able to achieve an optimum accuracy of 84.70% without use of GPU or more desired RAM.
### For Testing-
For testing,any image provided to the model can be predicted if the image is of either of the two person's faces. The testing can also be done through the Web Cam of the laptop/PC. 

## How to run this project?   
### Step-1    
--> Pull the code "Face Recognition dataset using CV2 & Haar Cascade" from this GitHub repository and run the code (say in Jupyter Notebook). By running the code, your Webcam will be switched on and it will take 1000 pictures of your face and save it in the specified folder by you. I have put up code for making face dataset of 2 people, you can change it according to your requirement.
### Step-2
--> Pull the code "Transfer Learning code for VGG16" from this GitHub repository and run it, this code will train a model for the face detection of the dataset that you have created in Step-1. This code is of transfer learning and the pre-trained model I have used to transfer the learning to my face model is of VGG-16. This code will detect whose face it is among the faces trained. This way we can detect faces easily.

## Scope of improvement
I'm trying to improve the accuracy of the model to more higher level.

## Acknowledgement
I would like to thank **Mr. Vimal Daga Sir** for teaching us the concepts so clearly and deeply.


