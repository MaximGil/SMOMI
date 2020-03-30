# SMOMI Отчет о лабораторной работе №2
В файле изначально были изменены: lr = 0.000000001, BUTCH_SIZE = 1, NUM_CLASSES = 2
Произвел 87 эпох.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_loss.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_val_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_val_loss.png)
Добавил один слой  
tf.keras.layers.Conv2D(filters=8, kernel_size=3),
        tf.keras.layers.MaxPool2D()
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_loss.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_val_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_val_loss.png)
        
