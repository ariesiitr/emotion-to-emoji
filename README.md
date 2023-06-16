# Emotion_To_Emoji
# PROJECT AIM:
Our project aims to develop a model that takes a person's video as input and displays the emotion using an emoji. This model uses deep learning concepts to recognize the emotion of one or multiple people at a time.
# To access our project:
you have to first download jupyter notebook and Python on your device . Download the dataset using this link  https://www.kaggle.com/datasets/msambare/fer2013. Then download the codes: MODEL.ipynb has the code for training the model, and OpenCV.ipynb has the code for using OpenCV and Flask framework. Then you have to download the pre-trained models if you don't want to train them by yourself; the links are provided at the end of the spec doc, and when and where to use them is specified in the code in the form of comments. Also, you have to download the uploaded emoji folder and update the emoji path from our code to yours. Finally, you need to run the openCV.ipynb file after updating all paths, you will get an address of a web app, copy it, and open it in a new window. Rest instructions are provided in the code in the form of comments.
# BRIEF WALKTHROUGH:
 ● LOADING THE APPROPRIATE DATA SET CONTAINING SUFFICIENT IMAGES OF
 ALL 7 TYPES OF EMOTIONS
 ● DATA AUGMENTATION AND IMAGE PRE-PROCESSING USING
 “ImageGenerator” and “.flow_from_directory”
 ● BUILDING THE CNN ARCHITECTURE
 ● COMPILING OUR MODEL USING LOSS, OPTIMIZERS (Adam) & METRICS
 ● TRAINING OUR MODEL WITH A TRAINING SET AND SAVING OUR MODEL
 ● EVALUATING TESTING ACCURACY
 ● USING OPENCV WHICH IS A REAL-TIME COMPUTER VISION LIBRARY TO
 CAPTURE THE VIDEO USING THE APPROPRIATE FRAME
 ● MAPPING THE EMOJIS WITH THE HIGHEST PROBABLE EMOTION
 ● USING FLASK FRAMEWORK TO BUILD A WEBPAGE
