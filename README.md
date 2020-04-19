Лабораторная работа №4
BUTCH_SIZE = 8, lr = 10^(-11)
a) горизонтальное отражение

![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/flip.png)

b) Аугментация с помощью поворота на случайный угол [-a;a]. Файл train_rotate.py
   30 градусов 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/rotate_30.png)
 
   45 градусов 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/rotate_45.png)

c) аугментация данных с помощью случайного изменения яркости и контраста. Файл train_brigth.py        

     tf.image.random_brightness(image, 0.4, seed=None)
     tf.image.random_contrast(image, 0.2, 1.2 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/brigth_1.2.png)

     tf.image.random_brightness(image, 0.5, seed=None) 
     tf.image.random_contrast(image, 0.3, 1.3 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/brigth_1.3.png)

     tf.image.random_brightness(image, 0.6, seed=None)
     tf.image.random_contrast(image, 0.4, 1.4 seed=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/brigth_1.4.png)
d) Аугментация с использованием случайного участка изображения

    tf.image.random_crop(image, size=[170, 130, 3], seed=None, name=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/crop_170.png)
       
    tf.image.random_crop(image, size=[112, 112, 3], seed=None, name=None)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/crop_112.png)

e) Методы a, b, c, d с оптимальными параметрами

    image = tf.image.random_crop(image, size=[112, 112, 3], seed=None, name=None)
    image = tf.image.random_flip_left_right(image)
    image = tf.image.random_brightness(image, 0.6, seed=None)
    image = tf.image.random_contrast(image, 0.4, 1.4, seed=None)
    degree = 45
    dgr = random.uniform(-degree, degree)
    image = tf.contrib.image.rotate(image, dgr * math.pi / 180, interpolation='BILINEAR')
    
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab4/CNN-XRay/lab4/all_augment.png)
