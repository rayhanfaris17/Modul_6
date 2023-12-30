# Rock Paper Scissors Image Classification
This project using VGG19 an advanced Convolutional Neural Network (CNN) for image classification of rock, paper, and scissors hand gestures. The model is trained using the Keras library and deployed as a web application using Flask.

## Dataset
The dataset consists of images of hand gestures representing rock, paper, and scissors. The dataset is divided into training, validation, and test sets.

![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/rock1.png)
![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/paper1.png)
![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/scissors.png)

## Model Architecture

This is the result of VGG19 model:

![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/vgg19%20model.png)

## Training

The model is trained for 3 epochs using the training dataset. The training progress is monitored, and the learning rate is reduced by a factor of 0.5 if there is no improvement in validation accuracy for 2 consecutive epochs.
and then the model save to .h5 file

## Evaluation

Graph Training and Validation Accuracy :

![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/acc.png)

Graph Training and Validation Loss :

![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/loss.png)

Classification Report

              precision    recall  f1-score   support

       paper       0.97      1.00      0.99        67
        rock       1.00      1.00      1.00        82
    scissors       1.00      0.99      0.98        86
    accuracy                           0.99       235
    macro avg      0.99      0.99      0.99       235
    weighted avg   0.99      0.99      0.99       235

## Result

![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/result1.png)
![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/result2.png)
![pictures](https://github.com/rayhanfaris17/Modul_6/blob/main/pictures/result3.png)


## Web Deployment

The trained model is deployed as a web application using Flask. Users can upload an image, and the model will predict whether the hand gesture represents rock, paper, or scissors.

```bash
python app.py
```

Visit http://localhost:5000/ in your web browser to use the application.



