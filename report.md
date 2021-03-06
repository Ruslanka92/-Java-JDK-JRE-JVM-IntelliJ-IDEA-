# Отчёт о тестировании <Задача №1 - Credit Card Number Validator>

## Краткое описание

<04.07.2021> - <04.07.2021> было проведено <тестирование методом чёрного ящика> приложения <Задача №1 - Credit Card Number Validator>.

На тестирование затрачено: <2 часа>

В результате тестирования выявлены следующие дефекты:
* <Не валидны карты AmericanExpress количество цифр номера - 15 шт.>
* <Не валидны карты VISA и Voyager количество цифр номера - 13 шт.>
* <Не валидны карты Diners Club количество цифр номера - 14 шт.>

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* <тест-план валидатора номера карты>

### тест-план валидатора номера карты
1. Валидный ввод номера карты [16 цифр]
1. Пустой ввод
1. Ввод 1 цифры
1. Ввод 15 цифр
1. Ввод 17 цифр
1. Ввод 1 пробела
1. Ввод 1 пробела и 15 цифр
1. Ввод 15 цифр и 1 пробела
1. Ввод 16 пробелов
1. Ввод 1 буквы и 15 цифр
1. Ввод 15 букв и 1 цифры
1. Ввод 16 букв
1. Ввод 1 специального символа и 15 цифр
1. Ввод 15 специальных символов и 1 цифры
1. Ввод 16 специальных символов

В качестве тестовых данных использовались данные <указать источник, откуда брались тестовые данные>:
* <Валидный ввод номера карты [16 цифр] - Result is OK>  (https://www.businessyeti.com/Apps/CreditCardGenerator/)
* <Пустой ввод - Result is FAIL> 
* <Ввод 1 цифры - Result is FAIL>
* <Ввод 15 цифр - Result is FAIL>
* <Ввод 17 цифр - Result is FAIL>
* <Ввод 1 пробела - Result is FAIL>
* <Ввод 1 пробела и 15 цифр - Result is FAIL>
* <Ввод 16 пробелов - Result is FAIL>
* <Ввод 1 буквы и 15 цифр - Result is FAIL>
* <Ввод 15 букв и 1 цифры - Result is FAIL>
* <Ввод 16 букв - Result is FAIL>
* <Ввод 1 специального символа и 15 цифр - Result is FAIL>
* <Ввод 15 специальных символов и 1 цифры - Result is FAIL>
* <Ввод 16 специальных символов - Result is FAIL>

Тестирование производилось в следующем окружении:
* <Windows 10 домашняя 64 разрядная>
* <Java 11.0.11>
