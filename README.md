# Rock Paper Scissors Image Classification
This project using VGG19 an advanced Convolutional Neural Network (CNN) for image classification of rock, paper, and scissors hand gestures. The model is trained using the Keras library and deployed as a web application using Flask.

## Dataset
The dataset consists of images of hand gestures representing rock, paper, and scissors. The dataset is divided into training, validation, and test sets.

![rock01-000](https://github.com/briliando00/RPS-Predict/assets/71593813/6478068d-9369-4241-8e5f-da0937ff3967)
![paper01-000](https://github.com/briliando00/RPS-Predict/assets/71593813/4fefa0da-e827-498e-9998-2db098b35b5d)
![scissors01-000](https://github.com/briliando00/RPS-Predict/assets/71593813/088b9324-30c7-41ea-8bd7-531b2a767b76)

## Model Architecture

This is the result of VGG19 model:



## Training

The model is trained for 3 epochs using the training dataset. The training progress is monitored, and the learning rate is reduced by a factor of 0.5 if there is no improvement in validation accuracy for 2 consecutive epochs.
and then the model save to .h5 file

## Evaluation

Graph Training and Validation Accuracy :

![image](https://github.com/briliando00/RPS-Predict/assets/71593813/abf13374-81c5-44d0-bdf1-deacf3b909b2)

Graph Training and Validation Loss :

![image](https://github.com/briliando00/RPS-Predict/assets/71593813/d7887e7b-0342-4f07-a6fa-326ac567f38a)

Classification Report

              precision    recall  f1-score   support

       paper       0.97      1.00      0.99        67
        rock       1.00      1.00      1.00        82
    scissors       1.00      0.99      0.98        86
    accuracy                           0.99       235
    macro avg      0.99      0.99      0.99       235
    weighted avg   0.99      0.99      0.99       235

## Result

![image](https://github.com/briliando00/RPS-Predict/assets/71593813/b5eda0c8-46e7-4e0d-9946-862234788897)


## Web Deployment

The trained model is deployed as a web application using Flask. Users can upload an image, and the model will predict whether the hand gesture represents rock, paper, or scissors.

```bash
python app.py
```

Visit http://localhost:5000/ in your web browser to use the application.



