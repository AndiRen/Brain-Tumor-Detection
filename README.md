# Examing the Robustness of Transfer Learning in Brain Tumor Diagnosis

## Overview

-Compares two self-built deep nerual networks with a transfer-learning model built on the EfficientNetV2B2 model.    
-All three models performed above 0.9 in both accuracy and macro F1 on the test data set.  
-However, when using a new data set of similar brain scan images, but with some novel orientations, the pretraiend model vastly outperformed the self-built models.  
-[The Br35H :: Brain Tumor Detection 2020](https://www.kaggle.com/datasets/ahmedhamada0/brain-tumor-detection) Kaggle data set was used to train and do inital testing of the models.  
-[The Brain Tumor Classification (MRI)](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri?select=Training) Kaggle data set was used to retest the models on similar, but new brain scan data.

## Results on Initial Training Set

### Self-Built Small-Scall Convolusion Neural Netowrk  
-*accuracy*: 0.9300  
-*macro F1*: 0.9344  

### Self-Built Residual Neural Network
-*accuracy*: 0.9400  
-*macro F1*: 0.9432  

### Pretrained Model Based on EfficientNetV2B2
-*accuracy*: 0.9233  
-*macro F1*: 0.9235  

## Results on Novel Training Set

### Self-Built Small-Scall Convolusion Neural Netowrk  
-*accuracy*: 0.7907  
-*macro F1*: 0.7990  

### Self-Built Residual Neural Network
-*accuracy*: 0.6116  
-*macro F1*: 0.6981  

### EfficientNetV2B2 Out of the Box
-*accuracy*: 0.8775  
-*macro F1*: 0.8631  

### Pretrained Model Based on EfficientNetV2B2
-*accuracy*: 0.9527  
-*macro F1*: 0.9432  

## Conclusions

1. Transfer learning ideal for quick, cheap, and robust prototyping.  
2. Can use prototyping to investigate research goals and identify data needs.  
3. Once research goals and data needs identified can build infrastructure necessary to effectively train specialized models.  
