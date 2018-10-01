# Tensorflow_API-Custom_object_detection
A sample project to detect custom object using Tensorflow object detection API

## Folder Structure
- Tensorflow_API-Custom_object_detection
  - dataset
    - Annotations
      - *Annotations for your images comes here*
    - JPEGImages
      - *all of your images for training comes here*
    - testImages
      - *all your images for testing comes here*
    - lable.pbtxt
    - train.record
   - output
     - *inference graph will be saved here*
   - train
     - *checkpoints will be saved here*
   - eval.ipynb
   - train.ipynb

## Steps

###### Create folders
Create the folders following the structure given above

###### prepare train and test images
This repository contains train and test images for detection of "UE Roll" blue bluetooth speaker but I will highly recommend you to create your own dataset. Pick up an object you want to detect and take some pics of it with varying backgrounds, angles and distances.  Sample of images used in this sample project is given below:

![img-2861](https://user-images.githubusercontent.com/5885636/46312084-b2084500-c5e1-11e8-909d-b9946b63343e.jpg)

Once you have captured pictures, transfer it to your PC and resize it to smaller size (given images have size of 605 x 454) so that your training will go smoothly without running out of memory. Now divide your captured images in to two chunks, one chunk for training and other for testing. Finally move training images in to *JPEGImages* folder and testing images in to *testImages* folder.

###### Label the data
Now its time to label your training data. We will be doing it using labelImg library. To download this library use [THIS LINK](https://github.com/tzutalin/labelImg). 
Once you have labelImg library downloaded on your PC, run lableImg.py. Select *JPEGImages* directory by clicking on *Open Dir* and change your save directory to *Annotations* by clicking on *Change Save Dir*. Now all you need to do is to draw rectangles around the you are planning to detect after clicking on *Create RectBox* and save it so that Annotations will get saved as .xml file in *Annotations* folder. 

![screenshot 2018-10-02 01 08 08](https://user-images.githubusercontent.com/5885636/46311801-eb8c8080-c5e0-11e8-8444-aa45e39b1414.png)

___________Under progress _____________


