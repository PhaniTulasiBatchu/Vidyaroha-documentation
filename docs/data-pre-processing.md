<style>
body{
background-color:rgb(34, 32, 32);
}
</style>

#<span style="color:rgb(212, 209, 253);">What is DATA PRE- PROCESSING ?</span>
<p style="color:rgb(150,150,150); font-weight:100;"><i><b>Data Pre-Processing </b></i>are techniques that involves transforming raw data into an understandable format. Real-world data is often incomplete, inconsistent, noisy and lacks certain behaviors or attributes, and is likely to contain many errors and imperfections. So data preprocessing is a proven method of resolving such issues.
<br>The Data we are having in this project is in the form of images. So we will be dealing with image pre-processng techniques, which are sub-sets of data preprocessing.
<br><i><b>Image preprocessing</b></i> are the steps taken to format the images before they are loaded into training models which includes, image resizing, scaling, color corrections and many more.</p>
<br>

#<span style="color:rgb(212, 209, 253);">Why do we need it ?</span>
<p style="color:rgb(150,150,150); font-weight:100;">The data that we receive might not always be in the best form to feed in to the model. Hence to just manipulate the data to the form we can use effectively, we perform data preprocessing.Two things play a very important role in the face recognition pipeline. The first being the pose and second is the lighting conditions (illumination).

Problem identified in the dataset given to us: The images had different lighting conditions. When the pipeline would be deployed, we still have no control over the illumination. Hence we need to pre process our data so that all of the images would come to a common lighting condition.
The techniques we tried for achieving the same are:<br>
* Histogram equalizer<br>
* Adaptive Histogram equalizer (CLAHE) for grayscale images<br>
* CLAHE - by extracting each of the channels and equalising each channel<br>
* CLAHE - by equalising the ‘V’ channel of the HSV form of the image.<br>
* Logarithmic transform<br>
* Gamma Correction <br>
* Image specific Gamma Correction<br>
</p>
<br>
#<span style="color:rgb(212, 209, 253);">Concepts Explored</span>
<br>
##<span style="color:rgb(150,150,150); font-weight:bold;">1. Histogram Equalizer </span>
<p style="color:rgb(150,150,150); font-weight:100;">Histogram Equalization is a technique used to improve the contrast in images. The regions of lower contrast are improved to a higher contrast. The main objective of Histogram equalizer is to normalise the varying illumination conditions. 
Histogram Equalization can be applied to the whole image by equalizing the individual channels or by converting the image to another colour space.

Adaptive Histogram Equalizer or CLAHE is used to equalize the image at every section. We can set a particular clip limit value according to which the image will be normalized.

For this dataset we have used CLAHE by equalizing the ‘V’ channel of the HSV form of the image. Converting to HSV and then equalising gave the best results as compared to grayscale or RGB.</p>

![scene](img2.PNG)

##<span style="color:rgb(150,150,150); font-weight:bold;">2. Gamma Correction</span>
<p style="color:rgb(150,150,150); font-weight:100;">Gamma correction is used to improve the contrast of an image based on its current lighting conditions, which implies that for each image we can apply a different value of gamma and normalize it. 

We classified the images into three categories based on the illumination
Overexposed : Images with very bright lighting condition
Underexposed : Images with dark lighting condition
Neutral : Images with a good lighting
  
Based on this classification we used different values of gamma to correct the images.
We classified the images based on the bright and dark thresholds and applied the gamma values as 2 for underexposed images and 0.3 for overexposed images. No gamma correction was done for neutral images. </p>
![scene](img3.PNG)


#<span style="color:rgb(212, 209, 253);">Concluding Remarks</span>
<p style="color:rgb(150,150,150); font-weight:100;">For better results we have used the following pipeline for preprocessing:</p>
![scene](img1.PNG)
<br>
#<span style="color:rgb(212, 209, 253);">References</span>
[refer](https://medium.com/@fanzongshaoxing/detect-face-in-bad-lighting-condition-using-color-histograms-2571df5fc53b
)
<br>
<br>
<br>
##<span style="color:rgb(150,150,150);">----TABLE OF CONTENT----</span>
<span style="color:#808080;">1.</span> [Home](index.md)<br>
<span style="color:#808080;">2.</span> [Overview](overview.md)     
<span style="color:#808080;">3.</span> [Introduction](introduction.md)    
<span style="color:#808080;">4.</span> [Data-pre-processing](data-pre-processing.md)   
<span style="color:#808080;">5.</span> [Face-Detection](face-detection.md)   
<span style="color:#808080;">6.</span> [Face-Alignment](face-alignment.md)    
<span style="color:#808080;">7.</span> [Face-Recognition](face-recognition.md)   
<span style="color:#808080;">8.</span> [Face-Verification](face-verification.md) 







