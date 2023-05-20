# Задание 4
На основе ноутбука с примером из лекции (segmentation.ipynb) написать свою версию Unet (заготовка для задачи - segmentation_by_hands.ipynb) - слои должны создаваться вручную, работа ведется с датасетом oxford_iiit_pet. Глобально менять архитектуру сети нельзя. Можно добавлять слои (но только вручную), менять функции активации, функцию ошибки, размеры batch и количество эпох. Цель - добиться от нейросети из segmentation_by_hands точности не ниже, чем для нейросети из segmentation при 20 эпохах.

1. Имортируем нужные библиотеки и подгружаем датасет  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_195758013.png)  

2. Загружаем и нормализуем изображения  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_233416091.png)  

3. Задаем параметры для обучения модели и загружаем обучающие и тестовые изображения  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_233709480.png)  

4. Расширение данных перед обучением модели  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_234024961.png)  

5. Визуализируем случайное изображение и его маску из обучающего набора данных  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_234242500.png)  

6. Прописываем какие слои будут в нашей модели U-Net и определяем её для сегментации изображений  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-20_235739199.png)  
![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000216884.png)  

7. Визуализация архитектуры модели  

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000252657.png) 

8. Создания маски сегментации и визуализация предсказаний модели на изображениях

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000356156.png)  
![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000417216.png)  

9. Обучение нашей модели   

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000555038.png)  

10. Итоговый результат   

![image info](https://github.com/misshp11/CV4/blob/main/img/изображение_2023-05-21_000640641.png) 
