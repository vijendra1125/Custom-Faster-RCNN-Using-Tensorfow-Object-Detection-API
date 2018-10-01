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
######Create folders
Create the folders following the structure given above

###### prepare train and test images
This repository contains train and test images for detction of "UE Roll" blue bluetooth speaker but I will highly recommend you to create your own dataset. Pick up an object you want to detect and take some pics of it with varing backgrounds, angles and distances.  Sample of images used in this sample project is given below:
*TODO::insert images here*
Once you have captured pictures, tranfer it your PC and resize it to smaller size (given images have size of 605 x 454) so that your training will go smoothly without running out of memory. Now divide your captured images in to two chuncks, one chunck for training and other for testing. Finally move training images in to *JPEGImages* folder and testing images in to *testImages* folder.

###Label the data
Now its time to label your training data. We will be doing it using labelImg library. To download this library use [THIS LINK](https://github.com/tzutalin/labelImg). Once you have labelImg library downloaded on your PC, run lableImg.py.
Select *JPEGImages* directory by clicking on *Open Dir*. and change your save directory to *Annotations* by clicking on *Change Save Dir*. Now all you need to do is to draw rectangles around the you are planning to detect and save it so that Annotations will get saved as .xml file in *Annotations* folder. 

___________Under progress _____________


