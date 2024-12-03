# Road Sign Image Understanding Project

## Project Overview
This project is a deep learning-based system designed to classify road sign images into categories such as **traffic light**, **stop sign**, **speed limit**, and **crosswalk**. Using a convolutional neural network (CNN), the model processes a dataset of labeled images and predicts the type of road sign.

I initialy planned to make this project using only OpenCV and no IA. As i didn't achieve to make a well working model, I radically changed my strategy and made an IA using tenserflow on Google Collab.


## Dataset Structure

- **Images**: Road sign images are stored in the `images/` folder.
- **Annotations**: Corresponding XML files with bounding boxes and labels are in the `annotations/` folder.
- Source : https://makeml.app/datasets/road-signs

### Folder Structure
/road_sign/
├── images/
├── image1.jpg
├── image2.png
└── ... 
├── annotations/ │
├── annotation1.xml │
├── annotation2.xml │
└── ...


### Viewing the Outputs
1. **Training Graphs**: 
   - ![image](https://github.com/user-attachments/assets/af4b7997-7074-4f67-b9a4-24eab15b68cb)


2. **Predicted Images**:
   - ![image](https://github.com/user-attachments/assets/605f5be6-97d7-4b61-9f36-35f016f73302)
  
   
## Steps in the Workflow
1. **Data Preparation**:
   - Parse XML files to extract image labels.
   - Preprocess images (resize to 128x128 and normalize pixel values).
   - Map labels to indices.

2. **Model Training**:
   - Train a CNN with convolutional and fully connected layers.
   - Use dropout layers to prevent overfitting.

3. **Evaluation**:
   - Evaluate performance on a test dataset (20% split).

4. **Visualization**:
   - Display graphs of training/validation performance.
   - Visualize predictions on test images.
  
   
# Possible improvement
   -When testing, i realized that There was to much images tagged as "SpeddLimit" by the programm. To improve it, i should reduce the number of speed limits in the dataSet compared to others categories. So that the model will less see them and more others.


