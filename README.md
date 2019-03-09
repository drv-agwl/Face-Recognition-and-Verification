# Face-Recognition-and-Verification

The Face Recognition and Verification model is built using Siamese Network with ResNet as base model. The model is trained on images of 5700 different identities, each training sample consist of three images, an anchor image, positive image (different image of same person as of anchor), a negative image (image of a different person than anchor). The 3 128 long encoding vectors are then used to calculate the triplet loss which is backpropogated to train the siamese network.

# Downloading Dataset and Preprocessing

- Download the dataset from the link - http://vis-www.cs.umass.edu/lfw/
- Unzip the zip file in the directory where the notebook FaceRecog2.ipynb is present
- Run all the cells of the "Loading Libraries and Exploring Dataset" section to load the dataset
- if "Out of Memory / all RAM used" error occurs, load the dataset in parts using list slicing, The code in the section is commented to     explain how to do the same.

# How to test on different Images

- Add the new images to the directory in which the code files are present
- Open the FaceRecog2.ipynb notebook and find the section "Testing the model"
- Change the names of the anchor image, positive image, negative image as per your image names
- Run all the cells of "Testing the model" section
- Observe the "Anchor-Positive" score and "Anchor-Negative Score".
- Low "Anchor-Positive" and a higher "Anchor-Negative" score suggests that Positive image is much more closer to Anchor image than Negative image 
