# Superstore-data-pipeline
# ETL процесс обработки датасета "Superstore" в Pentaho DI и его визуализация в Power BI

**Содержание:**

* [Обзор проекта](#Обзор-проекта)
* [Датасет](#Датасет)
* [Технологии, которые применялись](#Технологии-которые-применялись)
* [Визуализация](#Визуализация)
* [Выводы](#Выводы)
* [Инструкция по запуску Проекта](#инструкция-по-запуску-проекта)

## Обзор проекта
<img width="369" alt="Без имени" src="https://user-images.githubusercontent.com/121936498/212932652-92fb9ff2-c6c2-4853-bc2e-7937b38df68a.png">

В этом проекте мы сначала извлекаем данные из файла xls, который был скачан с Kaggle и предварительно размещен на GitHub. Затем мы  загружаем датасет с помощью Pentaho DI в первый слой базы данных PostgreSQL, осуществляя тем самым стейджинг. После этого очищаем данные, разбиваем на таблицы, составляем их них витрину данных. Также реализована возможность запуска указанного ETL процесса из командной строки и по расписанию. 

Результатом визуализации являются четыре дашборда в Power Bi. На первом из них можно увидеть сколько товаров продано, какая получена выручка и прибыль по годам и всего,  а также прирост этих показателей из года в год и графики. На втором дашборде представлены графики прибыли и выручки от реализации товаров в разбивке по сегментам или категориям товаров. В третьем – прибыль от продаж по категория и наименованиям товаров. На четвертом дашборде на карте размером кружков показаны выручка и прибыль в зависимости от штата, а также  виды используемой доставки. 

## Датасет

[Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

## Технологии, которые применялись

+ Pentaho Data Integration для организации ETL процесса 
+ PostgreSQL для хранения данных
+ Power Bi для визуализации

## Визуализация
### Дашборд №1
![1](https://user-images.githubusercontent.com/121936498/212933053-f1825729-2e27-4728-adec-7fa199a40e3c.jpg)

### Дашборд №2
![2](https://user-images.githubusercontent.com/121936498/212933074-963e6452-0a7e-48bd-906c-984b90d459bf.jpg)

### Дашборд №3
![3-1](https://user-images.githubusercontent.com/121936498/212933115-cc669731-9eca-4dd7-afef-8697e8d9ff4a.jpg)
![3-2](https://user-images.githubusercontent.com/121936498/212933144-b157eec1-e9f9-460f-92ab-a86fb0efeb40.jpg)

### Дашборд №4
![4](https://user-images.githubusercontent.com/121936498/212933161-2654a93a-5bbd-409b-ae51-df7f88ac71c3.jpg)

## Выводы

На основании полученной информации из датасета Superstore можно понять какие наименования  товары пользуются спросом, а какие нет. Посмотреть наименования и категории товаров, приносящих прибыль. По товарам, приносящим убыток, можно сделать вывод о необходимости из замены. Можно понять какой сегмент лучше развивать, какой вид доставки используется чаще всего, узнать географию продаж и делать предположения по дальнейшему развитию компании.

## Инструкция по запуску Проекта



