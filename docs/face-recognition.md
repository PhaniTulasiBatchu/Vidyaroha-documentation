<style>
body{
background-color:rgb(34, 32, 32);
}
</style>
#<span style="color:rgb(212, 209, 253);">Facenet</span>
<p style="color:rgb(150,150,150); font-weight:100;">FaceNet is a one-shot face recognition pipeline,it uses a deep convolutional network that directly learns a mapping from face images to a compact Euclidean multidimensional space where distances directly correspond to a measure of face similarity. Once this space has been produced, tasks such as face recognition, verification and clustering can be easily implemented using standard techniques with FaceNet compact 128-D embeddings as feature vectors.To train, they used triplets of roughly aligned matching / non-matching face patches. A triplet is nothing but a collection one anchor image, one matching image to the anchor image and one non-matching image to the anchor image. So the triplet loss minimises the distance between an anchor and a positive, both of which have the same identity, and maximises the distance between the anchor and a negative of a different identity.
In this step we encode the image into embeddings. Embeddings are high dimensional
vectors. For feature extraction we are using a Facenet model. FaceNet is a deep neural
network used for extracting features from an image of a person’s face. It was published in
2015 by Google researchers Schroff et al. FaceNet takes an image of the person’s face as
input and outputs a vector of 128 numbers which represent the most important features of a
face. In machine learning, this vector is called embedding. Basically, FaceNet takes a
person’s face and compresses it into a vector of 128 numbers. Ideally, embeddings of similar
faces are also similar. With the help of those embeddings we perform face classification.
</p>
<p style="color:rgb(150,150,150); font-weight:100;">In this project we used facenet ot get the 128-d embeddings from each of the input images.</p>
![scene](img14.png)
##<span style="color:rgb(150,150,150);">----TABLE OF CONTENT----</span>
<span style="color:#808080;">1.</span> [Home](index.md)<br>
<span style="color:#808080;">2.</span> [Overview](overview.md)     
<span style="color:#808080;">3.</span> [Introduction](introduction.md)    
<span style="color:#808080;">4.</span> [Data-pre-processing](data-pre-processing.md)   
<span style="color:#808080;">5.</span> [Face-Detection](face-detection.md)   
<span style="color:#808080;">6.</span> [Face-Alignment](face-alignment.md)    
<span style="color:#808080;">7.</span> [Face-Recognition](face-recognition.md)   
<span style="color:#808080;">8.</span> [Face-Verification](face-verification.md) 