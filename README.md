# Gesture Recognition Model building

The notebook can be executed in both Google colab and Jarvis Lab. Both has different versions of Keras hence minor change is required to run in colab.


## Experiment 1 - Conv3D Without Data Augmentation
Best Model : model-00015-0.02074-1.00000-0.61517-0.80000
Total params: 1,734,661
Trainable params: 1,734,661
Non-trainable params: 0

Training Accuracy : 100%     Validation Accuracy : 80%
Observation : Training accuracy is way higher than the validation accuracy indicates the model is overfitting.


## Experiment 2 - Conv3D  Data Augmentation
Best Model : model-00010-0.53373-0.79186-0.83507-0.63000.keras
Total params: 1,734,661
Trainable params: 1,734,661
Non-trainable params: 0

Training Accuracy : 79%     Validation Accuracy : 63%
Observation : Difference between training accuracy and validation accuracy is reduced. This indicates that the overfitting is reduce with data augmentation.  

## Experiment 3 - Conv3D with Data Augmentation and additional Layer
Best Model : 
Total params: 1,734,589
Trainable params: 1,734,589
Non-trainable params: 0


## Experiment 4 - CNN 2D and RNN (LSTM) with Data Augmentation
Best Model : 

## Experiment 5 - CNN 2D and RNN (GRU) with Data Augmentation
Best Model : 

## Experiment 6 - Transfer Learning with MobileNet pre-trained model with Data Augmentation
Best Model : 


