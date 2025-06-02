# NN model to classify pictures of musical instruments
This is a repository to train the NN model using Conv2D and MaxPooling2D to recognize 10 types of musical instruments as shown below. This model might have more room for improvement as the model currently has an overall accuracy of **55%** after evaluation.

![music instruments](https://github.com/rizkyfernanda/P3---Musical-Instruments-Classification/blob/main/graphs/instr_images.png)

## NN model template:

| Layer (type)                    | Output Shape           |       Param # |
|---|---|---|
| conv2d (Conv2D)                 | (None, 128, 128, 32)   |           896 |
| max_pooling2d (MaxPooling2D)    | (None, 64, 64, 32)     |             0 |
| conv2d_1 (Conv2D)               | (None, 62, 62, 64)     |        18,496 |
| max_pooling2d_1 (MaxPooling2D)  | (None, 31, 31, 64)     |             0 |
| conv2d_2 (Conv2D)               | (None, 29, 29, 128)    |        73,856 |
| max_pooling2d_2 (MaxPooling2D)  | (None, 14, 14, 128)    |             0 |
| flatten (Flatten)               | (None, 25088)          |             0 |
| dense (Dense)                   | (None, 64)             |     1,605,696 |
| dense_1 (Dense)                 | (None, 10)             |           650 |

 - Total params: 1,699,594 (6.48 MB)
 - Trainable params: 1,699,594 (6.48 MB)
 - Non-trainable params: 0 (0.00 B)
 - Total params: 1,699,594 (6.48 MB)
 - Trainable params: 1,699,594 (6.48 MB)
 - Non-trainable params: 0 (0.00 B)

## Actual vs predicted - image preview
![Actual vs. predicted - preview](https://github.com/rizkyfernanda/P3---Musical-Instruments-Classification/blob/main/graphs/actual_vs_predict.png)

## Actual vs predicted - confusion matrix
![Confusion matrix](https://github.com/rizkyfernanda/P3---Musical-Instruments-Classification/blob/main/graphs/confusion_matrix.png)

# Dataset Source
Gegenava, N. (2022). Musical Instruments - A Global Collection of Iconic Musical Instruments for Image Classification. Kaggle. https://www.kaggle.com/datasets/nikolasgegenava/music-instruments (Accessed on May 26, 2025)

License: Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)
