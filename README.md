# Gesture Recognition Model building

The notebook can be executed in both Google colab and Jarvis Lab. Both has different versions of Keras hence minor change is required to run in colab.

The dataset can be downloaded from here - https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL


## Experiment 1 – With Conv3D model
Designed Conv3D model with four convolutional layers, and two dense hidden and an output layer with the following parameter count.

`Total params: 1,734,661
Trainable params: 1,734,661
Non-trainable params: 0`

Training Result :- Average Training Accuracy : 55%     Validation Accuracy : 35%
Decision + Explanation : Training accuracy is way higher than the validation accuracy indicates the model is overfitting and validation performance also less

## Experiment 2 - Conv3D  with Data Augmentation
Second experiment carried out with same model with data augmentation on – like random transformations of images by resizing, cropping and normalizing, etc.

Training Result :-  Training Accuracy : 95%     Validation Accuracy : 75%
Decision + Explanation : Overall performance of both Train and Validation is increased drastically. But the  difference between training accuracy and validation accuracy still exists. This indicates the model is overfitting.

## Experiment 3 - Conv3D with Data Augmentation and additional Layer

Third experiment carried out with an additional convolutional layer and data augmentation on – like random transformations of images by resizing, cropping and normalizing, etc.

Training Result :-  Training Accuracy : 91%     Validation Accuracy : 80%
Decision + Explanation :  Training performance is reduced while the validation performance is increased. This  indicates the model now has optimal fit. 


## Experiment 4 - CNN 2D and RNN (LSTM) 
Fourth experiment carried out with Conv 2D and LSTM units

Training Result :-  Training Accuracy : 76%     Validation Accuracy : 25%
Decision + Explanation :  Performance of both train and test has reduced drastically.

## Experiment 5 - CNN 2D and RNN (GRU) with Data Augmentation
Fifth experiment carried out with Con 2D and GRU units 

Training Result :-  Training Accuracy : 58%     Validation Accuracy : 40%
Decision + Explanation :  Performance of both train and test has improved compared to Experiment 4 but overall performance is low.

## Experiment 6 - Transfer Learning with MobileNet pre-trained model with Data Augmentation
Sixth experiment is carried out with pre-trained model (MobileNet) with GRU units with the following parameter count:-

`Total params: 5,081,621
Trainable params: 5,081,141
Non-trainable params: 480`

Training Result :-  Training Accuracy : 96%     Validation Accuracy : 85%
Decision + Explanation :  Overall performance has improved with more number of parameter.

## Final Conclusion
The above experiment and its result shows Conv 3D with data augmentation gives the best performing model considering the number of parameters. Though Transfer learning model gives bit higher performance but the number of parameter is almost 4 times than the Conv 3D.
Hence choosing the best performing model from that experiment - model-00018-0.21707-0.91478-0.63865-0.80500.keras


