# SSD-object-Detection

Goal: The goal is to leverage an existing object detector model to automatically detect new class of objects, an application of transfer learning.

Performed in Google Colab Notebook using GPU.

### Dataset 
10 labeled images of the new class.

### Model baseline + finetuning: 
The model is an SSD (single shot multibox detector) object detetion with Resnet50 backbone with feature pyramid network.
Input Image size 640x640. 

Fined tune the WeightSharedConvolutionalBoxPredictor layer. 
SGD optimizer. 
total_loss equal to the sum of localization_loss and classification_loss. 

### Evaluation Metric
The Intersection over Union (IOU) 
