# SMOMI Отчет о лабораторной работе №2
В файле изначально были изменены: lr = 0.000000001, BUTCH_SIZE = 1, NUM_CLASSES = 2
Произвел 87 эпох.
Обучающая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_loss.png)
Тестовая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_val_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/stock%20file./epoch_val_loss.png)

Добавил один слой  
tf.keras.layers.Conv2D(filters=8, kernel_size=3),
        tf.keras.layers.MaxPool2D()
        Тестовая выборка 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_loss.png)
Обучающая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_val_categorical_accurancy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/add%201%20layer%20without%20changes/epoch_val_loss.png)
        
Та же конфигурация, уже с добавленным одним слоем , но изменены следующие параметры
optimizer=keras.optimizers.sgd(lr=0.000001, momentum=0.5)
Тестовая выборка 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.000001%2C%20momentum%3D0.5)%2C/epoch_categorical_accuracy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.000001%2C%20momentum%3D0.5)%2C/epoch_loss.png)
Обучающая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.000001%2C%20momentum%3D0.5)%2C/epoch_val_categorical_accuracy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.000001%2C%20momentum%3D0.5)%2C/epoch_val_loss.png)

Так же три слоя, но уже параметры оптимизатора вот такие
optimizer=keras.optimizers.sgd(lr=0.0000001, momentum=0.5)

Тестовая выборка 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.0000001%2C%20momentum%3D0.5)%2C/epoch_categorical_accurancy%20(1).png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.0000001%2C%20momentum%3D0.5)%2C/epoch_loss%20(2).png)
Обучающая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.0000001%2C%20momentum%3D0.5)%2C/epoch_val_categorical_accurancy%20(1).png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/optimizer%3Dkeras.optimizers.sgd(lr%3D0.0000001%2C%20momentum%3D0.5)%2C/epoch_val_loss%20(1).png)

Так же три слоя, но уже optimizer=keras.optimizers.sgd(lr=0.000000001, momentum=0.9)
        tf.keras.layers.Conv2D(filters=64, kernel_size=3),
        tf.keras.layers.MaxPool2D(),
        tf.keras.layers.Conv2D(filters=64, kernel_size=3),
        tf.keras.layers.MaxPool2D(),
        tf.keras.layers.Conv2D(filters=8, kernel_size=3),
        tf.keras.layers.MaxPool2D()
        
        Тестовая выборка 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/last%20changes/epoch_categorical_accuracy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/last%20changes/epoch_loss.png)
Обучающая выборка
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/last%20changes/epoch_val_categorical_accuracy.png)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab2/CNN-XRay/last%20changes/epoch_val_loss.png)
