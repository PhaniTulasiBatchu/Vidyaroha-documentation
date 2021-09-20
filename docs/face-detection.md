<style>
body{
background-color:rgb(34, 32, 32);
}
</style>

#<span style="color:rgb(212, 209, 253);">Face Detection</span>
<p style="color:rgb(150,150,150); font-weight:100;">In this step we will detect the faces in the given image. There are several models that perform this. Some of them we explored are.<br>
1. OpenCV Haarcascade<br>
2. Keras - CNN (Convolutional Neural Network)<br>
3. Face Recognition using Dlib<br>
4. MTCNN in Python<br></p>

#<span style="color:rgb(212, 209, 253);">OpenCV Haarcascade</span>
<p style="color:rgb(150,150,150); font-weight:100;">It is a machine learning based approach where a cascade function is trained from a lot of positive and negative images. Then, it can be used on any image we want to detect faces in. It is well known for being able to detect faces and face parts in an image, but can be trained to detect a vast majority of objects.</p>

#<span style="color:rgb(212, 209, 253);">MTCNN in Python</span>
<p style="color:rgb(150,150,150); font-weight:100;">MTCNN or Multi-Task Cascaded Convolutional Neural Network is unquestionably one of the most popular and most accurate face detection tools today. As such, it is based on a Deep learning architecture, it specifically consists of 3 neural networks (P-Net, R-Net, and O-Net) connected in a cascade.</p>
#<span style="color:rgb(212, 209, 253);">Concluding Remarks </span>
<p style="color:rgb(150,150,150); font-weight:100;">Out of these we used detecting faces with Facenet. Because it is very effective at detecting faces correctly. From facenet_pytorch we imported mtcnn and we used it to detect faces. After preprocessing the image we sent that image to mtcnn to detect the faces. After detecting the faces we are sending those faces for a feature extraction model to get embeddings.</p>
<br>
![scene](img4.PNG)
<br>
<br>
<br>
<br>
##<span style="color:rgb(150,150,150);">----TABLE OF CONTENT----</span>
<span style="color:rgb(212, 209, 253);">1.</span> [Overview](overview.md)         
<span style="color:rgb(212, 209, 253);">3.</span> [Data-pre-processing](data-pre-processing.md)   
<span style="color:rgb(212, 209, 253);">4.</span> [Face-Detection](face-detection.md)   
<span style="color:rgb(212, 209, 253);">5.</span> [Face-Alignment](face-alignment.md)    
<span style="color:rgb(212, 209, 253);">6.</span> [Face-Recognition](face-recognition.md)   
<span style="color:rgb(212, 209, 253);">7.</span> [Face-Verification](face-verification.md)   
<span style="color:rgb(212, 209, 253);">2.</span> [Conclusion](introduction.md)
