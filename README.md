# tools-classification

This repository aims to develop a robust algorithm to classify a dataset of tools available here : 
http://www.usine-agile.fr/datas/22-cnn-datas-1.html)
The database is divided into 5 parts : each part is a set of images of 7 different tools, but with different conditions. You can vizualise the images and the conditions in the jupyter notebook.

The first solution consists in using transfer learning. We use Keras and VGG16 CNN to extract features from the images, and then,
due to the limited number of images, we use a SVM to classify the images.

This first approach is a Supervised Learning problem. But the final aim is to have a solution that is able to detect novelties 
and to continuously learn. In fact the algorithm is aimed to be deployed for collaborative robots (colrobots).

The ultimate goal is to give a robot the abilty to classify the tools in a workspace, in order to help the human in their every day tasks.

Example :
Human : "give me the screwdriver!"
Robot has to recognize the screwdriver and to give it to the human.
