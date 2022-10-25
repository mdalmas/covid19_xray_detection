# Detecting COVID-19 in X-ray images with Keras & TensorFlow

Detecting COVID-19 in X-ray images with deeplearning using keras and tensorflow, Image classification.

## NOTE

This notebook was ran on google collab. As My gtx1050ti was unable to handle it.

### Prerequisites

Tensorflow 2.xx</br>
Keras</br>
h5py
## Details
1. **The dataset:**
   1.	The COVID-19 X-ray image dataset we’ll be using for this solution was curated by Dr. Joseph Cohen, a postdoctoral fellow at the University of Montreal.</br>
   2.	For healthy X-ray, we shall use   Kaggle’s Chest X-Ray Images (Pneumonia) dataset and sampled X-ray images from healthy patients.
2. **Pre-processing**
   1.	Extract the class label (either covid or normal) from the path 
   2.	Load the image, and pre-process it by converting to RGB channel ordering. 
   3.	Resizing the images to 224×224 pixels so that it is ready for our Convolutional Neural Network.
3. **Model**
   1. We used VGG16 model, along with our own model.
   2. Transfer learning, we initialized our model's top 2 convolutional layer's bais and weights of that of VGG16
4. **RESULT**
   1. On paper we got 98 % training and val accuracies BOTH,</br> Which is hard to believe as we only had 115 images of covid 19 positive patients.
   2. **Test** and training accuracies and losses</br>
   ![This was the results loss and accuracies](https://github.com/mdalmas/covid19_xray_detection/blob/master/plot.jpg)

### Using

***Just USE the notebook I don't not recommend using the .py file*** .<br>
I don't know what happens when you run the .py file.<br>
***Structure of folders is as uploaded***<br>

```
python covid19.py #ALTHOUGH I DON'T RECOMMEND BECUASE IT IS CONVERTED FROM .ipynb
```

You should get a trained model and a results plot at the end of the script.

### If you need my trained model <br>
.<a href="https://drive.google.com/drive/folders/1-MaL4eGaVyKz_1Ix_HCVs3VuvmEEoj1C?usp=sharing">  Download</a> <br>
contact me at almas.md60@outlook.com 


