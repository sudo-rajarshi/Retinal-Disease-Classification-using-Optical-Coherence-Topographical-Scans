This is a MULTICLASS CLASSIFICATION
20% data of the RAW Dataset is used for validation
10% data of the RAW Dataset is used for testing
The train dataset has 4 classes
The classes are = ['DME', 'DRUSEN', 'NORMAL', 'CNV']
The labels are:-
1 is labelled for DME
2 is labelled for DRUSEN
3 is labelled for NORMAL
0 is labelled for CNV


--HYPERPARAMETERS--
['Data is not Augmented']
Initial Learning Rate = 0.0001
Maximum No. of epochs = 100
Batch Size = 10
A model has been created at /home/rajarshi/Documents/OCT2017 


--MODEL-PARAMETERS--
Training Loss of the model has been monitored.
Activation Function = relu
Dropout = 30%
Activation function of the output layer = softmax
Cost function of the model = categorical_crossentropy
Optimizer = <keras.optimizers.Adam object at 0x7f0c962fff90>

Trained on a Custom Model
Number of layer = 5Number of Conv layer = 2
Filter size = 3*3

Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_1 (Conv2D)            (None, 128, 128, 16)      448       
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 128, 128, 16)      2320      
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 64, 64, 16)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 64, 64, 32)        4640      
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 64, 64, 32)        9248      
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 32, 32, 32)        0         
_________________________________________________________________
conv2d_5 (Conv2D)            (None, 32, 32, 64)        18496     
_________________________________________________________________
conv2d_6 (Conv2D)            (None, 32, 32, 64)        36928     
_________________________________________________________________
max_pooling2d_3 (MaxPooling2 (None, 16, 16, 64)        0         
_________________________________________________________________
conv2d_7 (Conv2D)            (None, 16, 16, 128)       73856     
_________________________________________________________________
conv2d_8 (Conv2D)            (None, 16, 16, 128)       147584    
_________________________________________________________________
max_pooling2d_4 (MaxPooling2 (None, 8, 8, 128)         0         
_________________________________________________________________
conv2d_9 (Conv2D)            (None, 8, 8, 256)         295168    
_________________________________________________________________
conv2d_10 (Conv2D)           (None, 8, 8, 256)         590080    
_________________________________________________________________
max_pooling2d_5 (MaxPooling2 (None, 4, 4, 256)         0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 4096)              0         
_________________________________________________________________
dense_1 (Dense)              (None, 256)               1048832   
_________________________________________________________________
dropout_1 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 4)                 1028      
=================================================================
Total params: 2,228,628
Trainable params: 2,228,628
Non-trainable params: 0
_________________________________________________________________

--MODEL-PERFORMANCE--
Training Accuracy = 99.92300271987915 %
Validation Accuracy = 94.11236047744751 %
Test Accuracy = 93.541818857193 %

Sensitivity = 98 %
Specificity = 95 %

Created using Self-Regulated Image Classifier using Convolution Neural Network