# RECOGNITION_OF_TAMIL_CHARACTERS_USING_CNN

### INTRODUCTION: 

"This repository contains a Convolutional Neural Network (CNN) tailored for recognizing handwritten Tamil 'Uyir Eluthu' characters. Trained on a dataset of handwritten samples, the model excels at accurately identifying and classifying these characters, offering a reliable solution for handwritten Tamil character recognition."

### MODEL ARCHITECTURE: 

Model: "sequential_18"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d_50 (Conv2D)          (None, 43, 43, 32)        320       
                                                                 
 max_pooling2d_48 (MaxPooli  (None, 21, 21, 32)        0         
 ng2D)                                                           
                                                                 
 conv2d_51 (Conv2D)          (None, 19, 19, 64)        18496     
                                                                 
 max_pooling2d_49 (MaxPooli  (None, 9, 9, 64)          0         
 ng2D)                                                           
                                                                 
 conv2d_52 (Conv2D)          (None, 7, 7, 128)         73856     
                                                                 
 max_pooling2d_50 (MaxPooli  (None, 3, 3, 128)         0         
 ng2D)                                                           
                                                                 
 flatten_16 (Flatten)        (None, 1152)              0         
                                                                 
 dense_32 (Dense)            (None, 128)               147584    
                                                                 
 dense_33 (Dense)            (None, 12)                1548      
                                                                 
=================================================================
Total params: 241804 (944.55 KB)
Trainable params: 241804 (944.55 KB)
Non-trainable params: 0 (0.00 Byte)
_________________________________________________________________

###EVALUATION: 
from classification report 
             precision    recall  f1-score   support

           1       0.74      0.88      0.80        16
           2       1.00      0.87      0.93        15
           3       0.86      0.63      0.73        19
           4       0.89      1.00      0.94        16
           5       0.82      0.88      0.85        16
           6       0.75      0.83      0.79        18
           7       0.68      0.87      0.76        15
           8       0.76      0.76      0.76        17
           9       0.77      0.67      0.71        15
          10       0.78      0.35      0.48        20
          11       0.46      0.75      0.57        16
          12       0.93      0.82      0.87        17

    accuracy                           0.77       200
   macro avg       0.79      0.78      0.77       200
weighted avg       0.79      0.77      0.76       200

###RESULTS: 
 The overall accuracy of the model, which is the ratio of correctly predicted instances to the total number of instances. In this case, the overall accuracy is 0.77 or 77%.
