# Face-Recognition-and-Verification

The Face Recognition and Verification model is built using Siamese Network with ResNet as base model. The model is trained on images of 5700 different identities, each training sample consist of three images, an anchor image, positive image (different image of same person as of anchor), a negative image (image of a different person than anchor). The 3 128 long encoding vectors are then used to calculate the triplet loss which is backpropogated to train the siamese network.

# How to test on different Images

- Add the new images to the directory in which the code files are present
- Open the FaceRecog2.ipynb notebook and find the section "Testing the model"
- Change the names of the anchor image, positive image, negative image as per your image names
- Run all the cells of "Testing the model" section
- Observe the "Anchor-Positive" score and "Anchor-Negative Score".
- Low "Anchor-Positive" and a higher "Anchor-Negative" score suggests that Positive image is much more closer to Anchor image than Negative image 
