# Capstone-Project-Honours

Report Abstract 

The project title is “Classification of Platelets using data from Totally Internal Reflective Fluorescent Microscopy (TIRFM)”. My name is Tegh Bir Singh and for the 2022 Spring semester I have been working on a way classify what stage a platelet is in. This is an important problem as it allows another way to quantify the effectiveness of a drug in terms of platelets and to better understand the behaviour of platelets better with respect drugs. 
However, the couple of problems that needed to be sorted before we can actually create an ML model. \

1.	Image data needs to be collected 
2.	The platelets need to be segmented before they can be classified 
3.	As the data is not labelled a way to label the data is needed for supervised machine learning 
4.	There are issues with classifying the platelets because the overlapping each other. 


The data has fortunately already been collected using TIRFM by Dr Qian Su.
  
To take of (2) we used a python package of cellpose. This creates outlines of the cells by using pre-trained neural network under the hood. 
Using the outlines of the platelet we are then able to get the user label what stage each platelet by assigning a number from 1-3 (integers only).
Ultimately, we unable to get the desired results when using support vector machine with low precision and recall of class 3. However, we identified problems with our approach. This offers the opportunity to use the work from this project as a framework for building an ML model.  


File Information:

- 221107 ML Platelets (Using SVM to classify platelets)
- 221107 File Processing Pipeline (Code is used to label the data)
- 221105 Data Visualisation (Contains data visualisation of TIF files. This is useful for labelling the data.)
