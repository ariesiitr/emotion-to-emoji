# Emotion_To_Emoji
# PROJECT AIM:
Our project aims to develop a model that takes a person's video as input and displays the emotion using an emoji. This model uses deep learning concepts to recognize the emotion of one or multiple people at a time.
# To access our project:
you have to first download jupyter notebook and Python on your device . Download the dataset using this link  https://www.kaggle.com/datasets/msambare/fer2013. Then download the codes: MODEL.ipynb has the code for training the model, and OpenCV.ipynb has the code for using OpenCV and Flask framework. Then you have to download the pre-trained models if you don't want to train them by yourself; the links are provided at the end of the spec doc, and when and where to use them is specified in the code in the form of comments. Also, you have to download the uploaded emoji folder and update the emoji path from our code to yours. Finally, you need to run the openCV.ipynb file after updating all paths, you will get an address of a web app, copy it, and open it in a new window. Rest instructions are provided in the code in the form of comments.
# BRIEF WALKTHROUGH:
 ● LOADING THE APPROPRIATE DATA SET CONTAINING SUFFICIENT IMAGES OF
 ALL 7 TYPES OF EMOTIONS \
 ● DATA AUGMENTATION AND IMAGE PRE-PROCESSING USING
 "ImageGenerator" and ".flow_from_directory" \
 ● BUILDING THE CNN ARCHITECTURE \
 ● COMPILING OUR MODEL USING LOSS, OPTIMIZERS (Adam) & METRICS \
 ● TRAINING OUR MODEL WITH A TRAINING SET AND SAVING OUR MODEL \
 ● EVALUATING TESTING ACCURACY \
 ● USING OPENCV WHICH IS A REAL-TIME COMPUTER VISION LIBRARY TO
 CAPTURE THE VIDEO USING THE APPROPRIATE FRAME \
 ● MAPPING THE EMOJIS WITH THE HIGHEST PROBABLE EMOTION \
 ● USING FLASK FRAMEWORK TO BUILD A WEBPAGE 
# MODEL:
 We used 2 different models - one is our customized model , we did some changes from a
 research paper to get maximum accuracy and other is vgg16 ( pre trained complex cnn
 model ) , we trained on both, vgg16 being complex and had more layers took a lot of time
 for even 20 epochs , but had almost same accuracy as our coustomized model.

# MAKING A GUI:
 After training the model and saving the labels in a .h5 file, we worked towards
 integrating the ML model with an interface like an app or webpage. We used flask framework
 for creating web application in python, to integrate the l model to web app. \
 After adding corresponding emotion's emoji to the frame, using imencode, we converted the
 image format of the frame to a streaming data format inthe  form of bytes of data to be
transferred over the net, then returned the frame to the main function call in the flask application,
 we usedthe  yield keyword that is used to return from a function without destroying the states of
 its local variable and when the function is called, the execution starts from the last yield
 statement. \
 Home function calls the mainpage.html file where the html framework is stored,
 which has a button that calls the function to start the camera view and emotion to
 emoji service, by getting the image view from the 'd' function defined using the flask
 fraework.\

 Rest details are in specdoc file
