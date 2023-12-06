# Вычисление оптического потока
> *Выполнила команда №5: **Набатов Арсений, Власенко Наталия, Ян Цзяфэн, Сёмочкин Владимир, Бурдаев Игорь***

## Подробное задание
https://github.com/tsjadambaa/cv_group6/tree/cv_lab6

## Архитектура нейронной сети
Поиск оптического потока выполнялся с помощью архитектуры нейронной сети FlowNetSimple.  

![image](https://github.com/4graf/optical_flow/assets/49661732/532b5d0b-9d9c-4fd7-b267-c08b179594aa)  

В отличии от оригинальной реализации FlowNetSimple датасет предобрабатывался путём сжатия фотографий к размеру **[192, 256]**.  
Данный подход позволяет уменьшить время обучения нейронной сети и время предсказания оптического потока, но в то же время точность 
предсказания снижается.



## Метрики

При заданных гиперпараметрах:
- Оптимизатор – **Adam(lr=0.0001)**
- Функция потерь – **EPE**
- Размер пакета – **4**
- Количество эпох – **20**

Метрики равнялись:
- Val Mean EPE – **8.73**
- Test Mean EPE – **7.34**
- Time per image – **0.013s**

## Картинки
### Train Validation EPE

![image](https://github.com/4graf/optical_flow/assets/49661732/ba60cbbc-9c8c-4bdc-9422-2a7c8f1478e9)

### Сравнение результатов

![image](https://github.com/4graf/optical_flow/assets/49661732/c082dbaf-1be7-4dee-a6f4-7005e66d7ec6)
![image](https://github.com/4graf/optical_flow/assets/49661732/f1808b85-02b6-4078-bfe6-36d3b9649620)
![image](https://github.com/4graf/optical_flow/assets/49661732/27c8014c-b054-428f-9f85-ed28ad5fa435)
![image](https://github.com/4graf/optical_flow/assets/49661732/43c13f1c-6252-4b0f-a603-d3a94bae408c)
![image](https://github.com/4graf/optical_flow/assets/49661732/537c611a-4d28-4357-819e-4fa7b957f4aa)
