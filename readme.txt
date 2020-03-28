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
Optimizer = <keras.optimizers.Adam object at 0x7f7c0c767510>


--MODEL-PERFORMANCE--
Training Accuracy = 99.82717633247375 %
Validation Accuracy = 96.01101875305176 %
Test Accuracy = 96.66906595230103 %

Classification Report:
              precision    recall  f1-score   support

         CNV       0.98      0.97      0.97      3720
         DME       0.90      0.94      0.92      1134
      DRUSEN       0.85      0.87      0.86       861
      NORMAL       0.96      0.95      0.96      2631

    accuracy                           0.95      8346
   macro avg       0.92      0.93      0.93      8346
weighted avg       0.95      0.95      0.95      8346

Sensitivity = 99 %
Specificity = 98 %

Created using Self-Regulated Image Classifier using Convolution Neural Network