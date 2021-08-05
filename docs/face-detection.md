<style>
body{
background-color:rgb(34, 32, 32);
}
</style>

#<span style="color:rgb(212, 209, 253);">Face Detection</span>
<p style="color:rgb(150,150,150); font-weight:100;">In this step we will detect the faces in the given image. There are several models that perform this. Some of them we explored are.<br>
1. OpenCV Haarcascade<br>
2. OpenCV DNN (Deep Neural Network)<br>
3. Detecting faces using Dlib<br>
4. Mtcnn in Python<br>
5. Detecting faces with Facenet</p>


<p style="color:rgb(150,150,150); font-weight:100;">Out of these we used detecting faces with Facenet. Because it is very effective at
detecting faces correctly. From facenet_pytorch we imported mtcnn and we used it to
detect faces. After preprocessing the image we sent that image to mtcnn to detect
the faces. After detecting the faces we are sending those faces for a feature
extraction model to get embeddings.</p>
<br>
![scene](img4.PNG)
<br>
#<span style="color:rgb(212, 209, 253);">Feature Extraction</span>
<p style="color:rgb(150,150,150); font-weight:100;">In this step we encode the image into embeddings. Embeddings are high dimensional
vectors. For feature extraction we are using a Facenet model. FaceNet is a deep neural
network used for extracting features from an image of a person’s face. It was published in
2015 by Google researchers Schroff et al. FaceNet takes an image of the person’s face as
input and outputs a vector of 128 numbers which represent the most important features of a
face. In machine learning, this vector is called embedding. Basically, FaceNet takes a
person’s face and compresses it into a vector of 128 numbers. Ideally, embeddings of similar
faces are also similar. With the help of those embeddings we perform face classification.</p>
<br>
#<span style="color:rgb(212, 209, 253);">Face classification</span>
<p style="color:rgb(150,150,150); font-weight:100;">In this step with the help of embeddings we are identifying the person in the image. There
are many classification algorithms like SVC,Logistic regression,KNN etc. We are using SVC,
cosine similarity and euclidean distance approach for classifying. In cosine similarity we will
find the cosine angle between two vectors. If the angle is less then the two images are the
same. In the euclidean approach we are finding the euclidean distance between two vectors.
If the distance is less then the both images are the same.</p>
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
