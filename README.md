# Hotel Image Classifier

This is a program that classifies the image, using tensorflow, supplied to it into categories: Bedroom, Livingroom, Kitchen, Bathroom, PropertyImage, SwimmingPool, along with providing a match percentage. 

It is build using TensorFlow framework. 

# Requirements

1. [docker](https://www.docker.com/products/docker-toolbox)
2. Tensorflow (https://www.tensorflow.org/versions/r0.9/how_tos/image_retraining/index.html, clone    from Github )
3. Python
4. Flask (Optional if you want to try to run the demo model)

# Usage
1. Download the code.
2. Run app.py through python in Terminal. 
3. Open the webpage it prompts in the Terminal.
4. Click on choose image and then select an image.
5. Upload the image.
6. Result will be shown in the next webpage.

A pre trained model will be required which can be found here: https://www.dropbox.com/sh/89v2jkbjagbkmul/AABDgww_Z2kTarwaNLN0kNjma?dl=0

Download these two file and update their path in the app.py code file. 

# Re-Training process

DataSet Creation

You just need to make a "classifier" directory with a directory "data" inside it with all your images
For example
```
 [any_path]/my_own_classifier/
 [any_path]/my_own_classifier/data
 [any_path]/my_own_classifier/data/Bedroom
 [any_path]/my_own_classifier/data/LivingRoom
 [any_path]/my_own_classifier/data/Kitchen
 [any_path]/my_own_classifier/data/Bathroom
 [any_path]/my_own_classifier/data/PropertyImage
 [any_path]/my_own_classifier/data/SwimmingPool
```
 and then put your image on it. 

NOTE: The data set should be as clean as possible for good results. Please keep this in mind. And bigger the data set the better.

 This "classifier" directory will have your samples but also trained classifier after execution of "train.sh". 

Re-train
 
You should have tensorflow repository cloned and all the files installed before running this. In the Retraining code folder, Just type
```
 ./train.sh [any_path]/my_own_classifier
``` 
A pre-trained model can be found here:  
https://www.dropbox.com/sh/89v2jkbjagbkmul/AABDgww_Z2kTarwaNLN0kNjma?dl=0

You can download the above two files and in the code change the
 
