># Аппаратура радиоуправления ArduFly 6
6 ти канальная аппаратура радиоуправления на базе Arduino.
* Радио модуль nRF20L01+
* Плата Arduino ProMini/Nano
* Возможность быстрой модернизации 
* Дальность 500-1500м

>## Подключение
* Правый горизонтальный стик (Елероны) - А0
* Правый вертикальный стик (Руль высоты) - А1
* Левый горизонтальный стик (Руль направления) - А2
* Левый вертикальный стик (Газ) - А3
* Правый потенциометр (5 канал) - А6
* Левый потенциометр (6 канал) - А7
* Правый двухпозиционный тумблер (Расходы) - 8
* Левый двухпозиционный тумблер (Арм мотора) - 6
* Бузер - 3
* Кнопка "Меню" - 7
* Кнопка "+" - 4
* Кнопка "-" - 5

>### Подключение nRF20L01+
![ArduFly](https://github.com/Viher-Sano/ArduFly_6/blob/master/images/nrf.PNG)

>## Инструкция 
Прошивка:
1. Скачайте и установите ArduinoIDE с сайта Arduino, установите драйвера для вашей платы.
2. Папку libraries переместите в папку C:/Users/Имя_Пользователя/Документы/Arduino
3. Откройте файл ArduFly_6.ino
4. Выберете порт к которому подключена ваша плата, а так же выберете из списка всех плат свою.
5. Нажмите кнопку загрузить. 
***
Что бы зайти в меню зажмите кнопку "Меню". 
Навигация по меню осуществляется кнопками "+" и "-".
***
Что бы настроить конечные точки:
1. Зайдите в меню зажатием кнопки "Меню" 
2. Выберете пункт "End points"
3. Выберете канал на котором нужно настроить конечные точки
4. Нажмите "Меню"
5. Кнопками "+" и "-" изменяйте значение (от 0 до 85)
6. Нажмите "Меню" что бы вернутся к выбору канала
7. Вернитесь в главное меню и выберете пункт "Save" что бы сохранить настройки
***
Что бы настроить реверс:
1. Зайдите в меню зажатием кнопки "Меню" 
2. Выберете пункт "Revers"
3. Выберете канал на котором нужно настроить реверс
4. Нажмите "Меню"
5. Кнопками "+" и "-" изменяйте значение ("ON" или "OFF")
6. Нажмите "Меню" что бы вернутся к выбору канала
7. Вернитесь в главное меню и выберете пункт "Save" что бы сохранить настройки
***
Что бы сбросить настройки:
1. Зайдите в меню зажатием кнопки "Меню" 
2. Выберете пункт "Default Settings"
5. Кнопками "+" и "-" изменяйте значение ("NO" или "YES")
4. Нажмите "Меню"
5. Дождитесь окончания очистки памяти.
>## Важно!!!
### Все настройки рекомендуется делать на земле!!!

>## Ссылки на комплектующие
* [16x2 LCD I2C](https://goo.gl/sR6fqJ)
* [Arduino Nano](https://goo.gl/ubKRwF)
* [Arduino ProMini](https://goo.gl/1xfWCh)
* [nRF20L01+](https://goo.gl/PhLPCz)
* [AMS 3.3v](https://goo.gl/Vu5vFW)
* [Переходник для nRF20L01+](https://goo.gl/mQg2Gd)

>## Что нового?

### v2.6
Добавлено: 
* Добавлена поддержка экрана 1602 I2C
* Многоуровневое меню (Вход по зажатию кнопки "Меню")
* Быстрая настройка конечных точек и реверсов
* Сохранение настроек в энергонезависимую память

Баги:
* Не работают двойные расходы 
****
### v2.7
Добавлено: 
* Автосохранение настроек
* Исправлен баг с двойными расходами
****
### v3.1
Добавлено: 
* Микширование каналов "Elevon"
****