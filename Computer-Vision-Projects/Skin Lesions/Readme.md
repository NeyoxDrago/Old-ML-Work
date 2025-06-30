A common task other than Object Detection and Object Classification in <B>Computer Vision</B> tasks is Object Segmentation.
<br> In this repository i have implemented segmentation of Skin lesions using UNET architecture in google colab. ( The code file contains link to colaboratory file. )
<br> The data was taken from ISIC 2018 challenge and contains around 2500 images with there respective segmentation files.

## Problems Faced while implementation
<br> Although i have ran it on google colab , with GPU enabled , i did faced som problems in implementing it , most were my systax problems .
<br> First problem was time it takes to run , currently it generates data for training by reading images in each epoch from the base directories , using a implemented custom generator. Thing i tried to improve this speed was , creating a combined numpy file of all these images but it took a huge amount of memory and hence due to which i wasn't 
<br> able to train my model  , hence i have to get it done in the older way.

<br> So currently it takes around 3-4 gb of ram and a huge of around 20 GB to keep the data.

## Results
Model recieved a accuracy score of 89% with a binary_crosentropy loss value as 0.3.
<br>Will get further improved by using BACKBONES or improving model architecture a bit.
<br>A sample result
![](https://github.com/NeyoxDrago/Object-Detection-Work/blob/main/Skin%20Lesions/download.png)

### Citation
<br>
<br> [1] Noel Codella, Veronica Rotemberg, Philipp Tschandl, M. Emre Celebi, Stephen Dusza, David Gutman, Brian Helba, Aadi Kalloo, Konstantinos Liopyris, Michael Marchetti, Harald Kittler, Allan Halpern: “Skin Lesion Analysis Toward Melanoma Detection 2018: A Challenge Hosted by the International Skin Imaging Collaboration (ISIC)”, 2018; https://arxiv.org/abs/1902.03368

<br> [2] Tschandl, P., Rosendahl, C. & Kittler, H. The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions. Sci. Data 5, 180161 doi:10.1038/sdata.2018.161 (2018).
