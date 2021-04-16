I. Introduction and Background
===================================
a. Introduction of DeepLabCut
----------------------------------------------
DeepLabCut is an advanced human pose estimation algorithm called DeeperCut can use relatively small amounts of annotated data in the lab. The main motivation of the DeePlabCut was to provide a reliable and effective tool for high-throughput video analysis, in this case learning about powerful user-defined feature detectors for body parts.

DeepLabCut has been used to extract user-defined locations of key body parts from animals (including humans).

DeepLabCut is best suited for one or more cameras to capture the action in one place with minimal occlusion. Users can train the network to achieve human-level marking accuracy with just a small group of training images, and extend its applications to behavioral analysis in the laboratory, such as for movement, gait analysis, medical and rehabilitation research.


b. The Backgroud of Project
--------------------------------------------
A species of fruit fly (drosophila melanogaster) is one of the most studied organisms in biological research, and has historically been used for genetic analysis in order to better understand other eukaryotic organisms, including humans. 

A research team at Kennesaw State University is currently developing a transparent omnidirectional motion compensator (TOLC) that allows flies to move indefinitely in a limited space, and errors in centroid calculations can degrade the performance of TOLC.

Currently, the team uses image segmentation to track the fly's center of mass.This method makes it difficult to define the area of the object, and results are inaccurate due to the movement of the fly.

The team is looking for a way to collect a more precise center of mass in images of Drosophila melanogaster. Our goal is to use DeeplabCut to greatly improve the speed and accuracy of tracking, which will allow KSU's research team to better study fly behavior. 

The current method the TOLC uses to predict the fly’s movement requires vulnerable morphological information (to detect the position and orientation of the fly) and error compensation (due to the distortion caused by the sphere). To remedy this, our team is using the software package DeepLabCut for animal pose estimation. DeepLabCut provides the ability to track desired features of an animal by means of transfer learning with deep learning networks that can achieve human-level accuracy with minimal training data.  

c. The Objective of Project
-----------------------------------------
The objective of our team's project is to train a network to recognize and track the center point (centroid) of the fruit fly. This is the point that the TOLC uses to determine how to orient the sphere. We manually labeled 100 frames out of a total of 60,984 to create a network that automatically places the centroid label on the fly. 

We used Drosophila Melanogaster for this project.The reason is that insects are commonly used for genetic investigations of humans and are considered to be one of the most perfect organisms for genetic patterns.

It is estimated that 60% of the fly genome is similar to the human genome.About 75% of human disease genes can be identified in fly genomes.Second, studying flies' behavior patterns could allow biologists and neuroscientists to better understand human behavior patterns.

Our secondary focus was to train a network that recognizes and places labels on each of the fly’s legs. For this network, we manually labeled 200 frames to ensure that we got the results we desired. While legs tracking is not used by the TOLC, we wanted to demonstrate the power and ease-of-use of the DeepLabCut toolbox. 

Finally, our work and trained networks will be provided to the development team behind the TOLC and will potentially be used in an enhanced version of the device. 
  
