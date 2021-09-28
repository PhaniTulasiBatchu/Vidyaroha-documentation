<style>
body{
background-color:rgb(34, 32, 32);
}
</style>
#<span style="color:rgb(212, 209, 253);">What is Face Alignment</span>
<p style="color:rgb(150,150,150); font-weight:100;">Face alignment is the process of identifying the geometric structure of different faces in digital images. We attempt to obtain a canonical alignment of the face based on translation, scaling, and rotation. There are many ways to perform face alignment. Some methods try to impose a (pre-defined) 3D model and then apply a transform to the input image such that the landmarks on the input face match the landmarks on the 3D model. Face alignment can be seen as a form of “data normalization”. Just as we normalize a set of feature vectors via zero cantering or scaling to unit norm, prior to training any model, we align the faces in our dataset before forwarding them in the pipeline. This process ensures higher accuracy from the face recognition models. </p>
#<span style="color:rgb(212, 209, 253);">Why do we need it</span>
<p style="color:rgb(150,150,150); font-weight:100;">We will be dealing with group images in this project. When a group image is captured, it may include positioning of several people in different angles, trying to face the camera with some degree of rotation in the face and other facial landmarks. In this case, there will be a loss in accuracy of the output due to these unnecessary rotations. So, we need to normalize these rotations in order to obtain better results when we move forward in the pipeline. </p>
#<span style="color:rgb(212, 209, 253);">Concepts Explored</span>
##<span style="color:rgb(150,150,150); font-weight:bold;">1. Face Alignment</span>
![scene](img6.PNG)
<p style="color:rgb(150,150,150); font-weight:100;">Face alignment is an early stage of the modern face recognition pipeline. Google declared that face alignment increases the accuracy of its face recognition model FaceNet from 98.87% to 99.63%. This is almost 1% accuracy improvement. Similar to face detection which is also the earlier stage of the pipeline, we can apply 2D face alignment within OpenCV in Python easily. </p>
![scene](img7.PNG)
##<span style="color:rgb(150,150,150); font-weight:bold;">2. Frontalization</span>
![scene](img8.png)
<p style="color:rgb(150,150,150); font-weight:100;">“Frontalization” is the process of synthesizing frontal facing views of faces appearing in single unconstrained photos. Recent reports have suggested that this process may substantially boost the performance of face recognition systems. This, by transforming the challenging problem of recognizing faces viewed from unconstrained viewpoints to the easier problem of recognizing faces in constrained, forward-facing poses. Previous frontalization methods did this by attempting to approximate 3D facial shapes for each query image. But here its observed that 3D face shape estimation from unconstrained photos may be a harder problem than frontalization and can potentially introduce facial misalignments. Instead, the simpler approach of using a single, unmodified, 3D surface as an approximation to the shape of all input faces is preferred. This leads to a straightforward, efficient and easy to implement method for frontalization. More importantly, it produces aesthetic new frontal views and is surprisingly effective when used for face recognition and gender estimation. </p>
![scene](img9.PNG)
##<span style="color:rgb(150,150,150); font-weight:bold;">Difference between the two</span>
<p style="color:rgb(150,150,150); font-weight:100;">The major difference is that in face alignment, we try to align a specific feature of the face , say eyeseither horizontally or vertically as per the users choice.No modifications are done to the structure of the face only the orientation is modified. Whereas in case of frontalization, the orientation is ignored and the modifications are made to the angle of tilt in the face so that any face tilted towards the right or left by any degree is turned back straight in such a way that all the facial features are visible in one frame. </p>
#<span style="color:rgb(212, 209, 253);">Contributors</span>
<p style="color:rgb(150,150,150); font-weight:100;">
1. Kodumuru Saketh<br>
2. Phani Tulasi Batchu<br>
</p>
#<span style="color:rgb(212, 209, 253);">References</span>
##<span style="color:rgb(150,150,150);">----TABLE OF CONTENT----</span>
<span style="color:rgb(212, 209, 253);">1.</span> [Overview](overview.md)         
<span style="color:rgb(212, 209, 253);">3.</span> [Data-pre-processing](data-pre-processing.md)   
<span style="color:rgb(212, 209, 253);">4.</span> [Face-Detection](face-detection.md)   
<span style="color:rgb(212, 209, 253);">5.</span> [Face-Alignment](face-alignment.md)    
<span style="color:rgb(212, 209, 253);">6.</span> [Face-Recognition](face-recognition.md)   
<span style="color:rgb(212, 209, 253);">7.</span> [Face-Verification](face-verification.md)   
<span style="color:rgb(212, 209, 253);">2.</span> [Conclusion](introduction.md)
