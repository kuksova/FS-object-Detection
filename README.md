# FS-object-Detection

Goal: The goal is to leverage an existing object detector model to automatically detect new class of objects, an application of transfer learning.

Performed in Google Colab Notebook using GPU.

### Dataset 
10 labeled images of the new class.

### Model baseline + finetuning: 
Few shot object detection model - fasterrcnn_resnet50_fpn_v2. (https://pytorch.org/vision/main/models/faster_rcnn.html)
Faster R-CNN model with a ResNet-50-FPN backbone.
Input Image size 480x640. 

Fined tune the WeightSharedConvolutionalBoxPredictor layer. 
SGD optimizer. 
total_loss equal to the sum of localization_loss and classification_loss. 

### Evaluation Metric
The Intersection over Union (IOU) 
