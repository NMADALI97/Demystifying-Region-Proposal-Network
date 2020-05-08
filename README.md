# Faster R-CNN for Open Images Dataset by Keras
## Introduction

I wrote my exploring and experiment results for Faster R-CNN in this  [article](https://medium.com/@nabil.madali/demystifying-region-proposal-network-rpn-faa5a8fb8fce). 

## Project Structure
`Object_Detection_DataPreprocessing.ipynb` is the file to extract subdata from Open Images Dataset V4 which includes downloading the images and creating the annotation files for our training. I run this part by my own computer because of no need for GPU computation. `frcnn_train_vgg.ipynb` is the file to train the model. The configuration and model saved path are inside this file. `frcnn_test_vgg.ipynb` is the file to test the model with test images and calculate the mAP (mean average precision) for the model. If you want to run the code on Colab, you need to give authority to Colab for connecting your Google Drive. Then, you need to upload your annotation file  and training images to the Google Drive and change my path to your right path in the notebook.

## Result for some test images
<p float="left">
    <img src="Assets/e2f4a864682b4645.jpg" width="425"/> 
    <img src="Assets/28cc7decbcc56aa1.jpg" width="425"/>
</p>
<p>
    <img src="Assets/96b74d5aaadc2259.jpg" width="425"/> 
    <img src="Assets/c3ca8496d6a9f2de.jpg" width="425"/> 
</p>

## Have fun

As the images shown below, they are three porcoelainous monks made by China. I just named them according to their face look (not sure about the sleepy one). They are definitely not included in the Open Images Dataset V4. Except for the three classes I used in Open Images Dataset V4, I create my own six-classes dataset ('Apple Pen', 'Lipbalm', 'Scissor', 'Sleepy Monk', 'Upset Monk' and 'Happy Monk') for fun and train another detector to find out these objects. If you want to know how to do this, just see this [article](https://medium.com/@rockyxu399/faster-r-cnn-object-detection-implemented-by-keras-for-custom-data-from-googles-open-images-125f62b9141a) for more details.
<p>
<img src="Assets/Result_customdata3.png" width="425"/>  
<img src="Assets/Result_customdata2.jpg" width="425"/> 
</p>
<img src="Assets/Result_customdata1.jpg" width="425"/>
