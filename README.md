# asl
American Sign Language recognition model 

A deep learning project where I trained a model over 80000 labeled images that classifies ASL letters, numbers, and control signs using EfficientNetB3 with a 99 percent test sccuracy.

#Overview:

The project uses CNN with a pretrained EfficientNetB3 to classify the ASL hand gestures in 39 categories:
1. Letter A-Z
2. Numbers 0-9
3. Special signs: 'space', 'delete', 'nothing'

The model was trained over the dataset: https://drive.google.com/file/d/1nQOzAf7ie77g3dZ5zOy9-R0C1hCYLx-l/view?usp=sharing

#Trained Model:

https://drive.google.com/file/d/1FXGbamnSGZ7wEGvgSGBmtp-FCEh2laPN/view?usp=sharing

#To predict:

Use the asl_test.py notebook to test the model on test images.
Ensure folder path and folder structure.
Replace or add new images in the test directory to evaluate more inputs.

#Training:

1. Trained over ~90K images and 30 epochs with validation split.
2. Used a T4 on colab.
3. Training Time: 2 hours.
4. First 200 layers were frozen for faster convergence and improved generalization.
