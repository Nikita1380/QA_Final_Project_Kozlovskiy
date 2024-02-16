﻿# Работа с базой данных
- Задание 1
- Необходимо проверить отображение созданного заказа в базе данных.
- Для этого: вывести список логинов курьеров с количеством их заказов в статусе «В доставке» (поле inDelivery = true). 
- Задание 2
- Необходимо убедиться, что в базе данных статусы заказов записываются корректно.
- Для этого: вывести все трекеры заказов и их статусы. 
- Статусы определяются по следующему правилу:
- Если поле finished == true, то вывести статус 2.
- Если поле canсelled == true, то вывести статус -1.
- Если поле inDelivery == true, то вывести статус 1.
- Для остальных случаев вывести 0.

# Автоматизация теста к API

- Клиент создает заказ.
- Проверяется, что по треку заказа можно получить данные о заказе.
- Шаги автотеста:
- Выполнить запрос на создание заказа.
- Сохранить номер трека заказа.
- Выполнить запрос на получения заказа по треку заказа.
- Проверить, что код ответа равен 200.

- Для запуска тестов должны быть установлены пакеты pytest и requests.
- Запуск всех тестов осуществляется командой pytest.