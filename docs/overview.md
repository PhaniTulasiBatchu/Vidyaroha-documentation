<style>
body{
background-color:rgb(34, 32, 32);
}
</style>
#<span style="color:rgb(212, 209, 253);">Purpose</span>
<p style="color:rgb(150,150,150); font-weight:100;">The prime purpose of doing this project is that we came across some deceiving practices as well as complications in the matter of marking attendance, which drove us towards an idea of using technology to solve this real world problem. Our major use case is Government schools and colleges which aim at providing aid, education and food to lakhs of students at free of cost. But there are many deceiving practices done by various officials, who misuse the benefits meant for those kids. And it is all possible by manipulating the attendance and getting the more out of it. So this is our attempt to turn down such actions, wherein we will be automating the attendance procedure by just needing the group image of students present in each class.</p>
#<span style="color:rgb(212, 209, 253);">Vision</span> 
<p style="color:rgb(150,150,150); font-weight:100;">We have done end-to-end face recognition which is the soul of  this project. And we used Amazon EC2 cloud services for configuring and deploying our project. A GUI is built which forms the home screen wherein the user needs to upload six different images of all the students in each and every class. After the upload is complete, the images are loaded into a particular folder and sent for training into the model. The model extracts a 128-d vector containing the facial landmarks in each face and stores it in a Database. Now a group image from which the attendance has to be taken is once again uploaded in the GUI, the given image is processed against the model by comparing the face embeddings of each face in the group image to that in the database and the output marks the attendance of the whole class which is again stored in a new database. We used MySQL for the database. This process can be iterated for different classes everyday making the attendance marking process easy and accurate. </p>
##<span style="color:rgb(150,150,150);">----TABLE OF CONTENT----</span>
<span style="color:rgb(212, 209, 253);">1.</span> [Overview](overview.md)         
<span style="color:rgb(212, 209, 253);">3.</span> [Data-pre-processing](data-pre-processing.md)   
<span style="color:rgb(212, 209, 253);">4.</span> [Face-Detection](face-detection.md)   
<span style="color:rgb(212, 209, 253);">5.</span> [Face-Alignment](face-alignment.md)    
<span style="color:rgb(212, 209, 253);">6.</span> [Face-Recognition](face-recognition.md)   
<span style="color:rgb(212, 209, 253);">7.</span> [Face-Verification](face-verification.md)   
<span style="color:rgb(212, 209, 253);">2.</span> [Conclusion](introduction.md) 
