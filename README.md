-----------------------------------------------------------------------------------------------
Name: Installing Tensorflow on Ubuntu 16.04 and Train the inception model.
 
Date Started: 09/08/17
 
Using:
Docker
Python 2.7
Android Studio
 
Why?
To check the extent of tensorflow for object detection and also to see if it works on ubuntu.
To train the inception v3 model with our custom images.


 
How?

Link 1 - https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/index.html#0
Firstly, one has to follow all the steps on this link to install the docker and tensorflow.

Then it will tell you to download flower images by default (you can use your own images)

Training the inception will be carried by the next step and it will put all the flower images on the last layer of the model so that it can only detect flowers.

Bottlenecks, retrained graph and retrained label files will be generated after training.

After that using python, one check that it is working or not.


Link 2 - https://codelabs.developers.google.com/codelabs/tensorflow-for-poets-2/#0
As per link 1, we have trained our inception model and we checked that the tensorflow is working or not.

Download tensorflow-for-poets-2 and copy the tf_files into it.

After following some basic steps about setting up docker and tensorflow then one need to optimize the tensorflow and the output will be optimized graph (speed up model with less calculations).

Compressing the model will generate another graph called rounded graph which is needed otherwise tensorflow won’t work.

Open it in Android Studio and Test.
 
Outcome
Tensorflow with our trained model works and  as we provided the model with flower photos it detects different types of flowers.
The confidence score is displayed on the top with the title.

 
Date Completed:  10/08/2017
 
What?
As it is live tracking, the camera optimizes itself every two seconds when detecting any new object.
After detecting the object, the one has the high confidence is displayed on the top.
 
Notes:
Try to follow each step properly and if you get stuck there is an link to a video at the end so you can look into it and follow.
 
Recommendation:
Train the inception for ant class.

---------------------------------------------------------------------------------------------------


Name: Trained the tensorflow app with ant class
 
Date Started: 08/08/17
 
Using:
Docker
Python 2.7
Android Studio
 
Why?
To check that tensorflow works with the trained inception model.
 
How?
Follow all the steps which is provided in the last spike.
Create a folder name “Ants” and another one named “Ants 2” and put all the images of it.
Use the links to train the inception model and provide the images of ants to it.
Train the model and check the confidence score by executing the python command.


 
Outcome
Downloaded the fire ant images and inserted into the tensorflow and trained the inception model with it.

Works fine but need to have two or more classes of objects (eg fire ants, red ants) otherwise it won't work.

 
Date Completed:  03/08/2017
 
What?
Live tracking is better because we can get understand the exact angle of total or close confidence score.
 
Notes:
When downloading the images, make sure no image is blank otherwise there will be an error regarding invalid JPEG file.
Also make sure to create a subfolder and then create two or more folders of ants otherwise there will be an error regarding “Classification”.
Refer the retrain.py file if there is any error.
 
