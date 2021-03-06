# MRI-based-brain-tumor-classification

This project detects and classifies brain tumor MRI images into three classes: Glioma tumor, Meningioma tumor, Pituitary and No tumor. Processed images are used to train convolutional neural networks to classify the images into four classes.


## Dataset:
Data can be downloaded from https://www.kaggle.com/sartajbhuvaji/brain-tumor-classification-mri


## Running the model:
The downloaded data folder should be placed inside the current foleder (where the code files exist) and named “data”. Before the next step, make sure the folder structure is Code --> Data --> Training, Testing.
Once the raw data is in place, go ahead and first run the jupyter file named “preprocessing.ipnyb”. This file will pre-process the data and automatically place the processed data folder (named “processed_data”) inside “data” folder.
Now the data is ready to be used in the models.

## Models
I experimented with different models. Following are the details of the model architectures showed better performance:
1. final-Nasnet: Uses NASNetMobile base architecture. 
2. final-Nasnet-balance-dataset: Model with class weights to balance the dataset
3. Inception: Uses Inception as the base mdoel.
4. RESNet - Uses Resnet50 as the base architecture.
