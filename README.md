# RECOGNITION_OF_TAMIL_CHARACTERS_USING_CNN

# INTRODUCTION: 

"This repository contains a Convolutional Neural Network (CNN) tailored for recognizing handwritten Tamil 'Uyir Eluthu' characters. Trained on a dataset of handwritten samples, the model excels at accurately identifying and classifying these characters, offering a reliable solution for handwritten Tamil character recognition."

# MODEL ARCHITECTURE: 

Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
conv2d (Conv2D)              (None, 43, 43, 32)        320
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 21, 21, 32)        0
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 19, 19, 64)        18496
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 9, 9, 64)          0
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 7, 7, 128)         73856
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 3, 3, 128)         0
_________________________________________________________________
flatten (Flatten)            (None, 1152)              0
_________________________________________________________________
dense (Dense)                (None, 128)               147584
_________________________________________________________________
dense_1 (Dense)              (None, 12)                1548
=================================================================
Total params: 241,804
Trainable params: 241,804
Non-trainable params: 0

#EVALUATION: 
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

#RESULTS: 
 The overall accuracy of the model, which is the ratio of correctly predicted instances to the total number of instances. In this case, the overall accuracy is 0.77 or 77%.
