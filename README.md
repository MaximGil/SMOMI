# SMOMI 
Нужно было построить полносвязную сеть из 5 слоев. Использовали один Flatten, и четыре Dense.
Количество нейронов в слоях Dense: 128,64,128,10.
Для первых трех слоев Dense использовали активатор "relu". а для последнего "softmax".
В обучении использовал метрику "acc", Обучение проходило в 23 эпохи. Использовали оптимизатор "adam".
Функция потерь SparseCategoricalCrossentropy.

Итоговая точность на обучающей выборке 0.4155

График метрики точности
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab1/epoch_acc)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab1/epoch_val_acc)

График функции потерь
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab1/epoch_loss)
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab1/epoch_val_loss)
