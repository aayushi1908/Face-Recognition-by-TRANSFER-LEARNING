# Face-Recognition-by-TRANSFER-LEARNING
Transfer Learning in Deep Neural Networks - The easiest way to describe transfer learning is the use of previously acquired knowledge and skills in new learning or problem-solving situations. 
I've divided this project into 2 parts-
1) For dataset creation- I've used Open-CV library and Haar Cascade classifiers for detecting the face. The dataset has been divided into two sets- train set and test set. For train set, the code captures 1000 images of the person's face. For the test set, the code captures 500 images of the person's face.
2) For training of VGG16 and testing the model - 
Firstly I've imported the VGG16 model and then its weights from ImageNet. In my new model, I have freezed all the intermediate layers of VGG except the Input and Output layer. I've trained the output layer according to my requirement. 
With the help of transfer learning, I'm able to achieve an optimum accuracy of 94.70% without use of GPU or more desired RAM.
For Testing, any image provided to the model can be predicted if the image is of either of the two person's faces. The testing can also be done through the Web Cam of the laptop/PC.

