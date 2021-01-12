###  Pneumonia-Chest-X-Ray-Images detection using Convolution Neural Network in Tensorflow
* The dataset can be downloaded from keggle webiste: https://www.kaggle.com/ryanawad/pneumonia-chest-x-ray-images-tensorflow
* two CNN models have been built:
  1. chest_image_CNN: A CNN model has been trained from scratch applying image augmentation method, and test data set has been used as validation data. 
With smaller batch size and multiple convolution layers, the model can achieve 92% of accuracy. This trained model can be used in future as transfer learning for other medical related image detection.
  2. chest_image_transfer: Transfer learning has been applied to this model. The pre-trained ResNet50 model has been used as base model. 
In the modeling process, only 30% of the training data has been used to combine with the pre_trained base model, however the model has the over fitting problem with the val_accuracy not improving.

