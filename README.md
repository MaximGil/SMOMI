Лабораторная работа №4

BUTCH_SIZE = 8, lr = 10^(-11)

a) горизонтальное отражение. File train_flip1.py

     image = tf.image.random_flip_left_right(image)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_flip1.png)

c) аугментация данных с помощью случайного изменения яркости и контраста. Файл train_brigth1.py        

     tf.image.random_brightness(image, 0.4, seed=None)
     tf.image.random_contrast(image, 0.4, 1.4 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_bright1_0.4.png)

     tf.image.random_brightness(image, 0.5, seed=None) 
     tf.image.random_contrast(image, 0.4, 1.4 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_brigth1_05.png)

     tf.image.random_brightness(image, 0.6, seed=None)
     tf.image.random_contrast(image, 0.4, 1.4 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_brigth1_06.png)
d) Аугментация с использованием случайного участка изображения

    tf.image.random_crop(image, size=[140, 140, 3], seed=None, name=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_crop1_140.png)
       
    tf.image.random_crop(image, size=[170, 170, 3], seed=None, name=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4_try2/CNN-XRay/lab4_remake/train_crop1_170.png)

