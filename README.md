# OOP
Функциональные требования для курсовой работы

Выполнил студент группы 353504 Шилов Андрей Валентинович 

Тема: Утилита для авто генерирования тестовых баз данных (Конвертер валют с базой данных)

Язык программирования: C#
База данных: MySQL

1. Основные функции утилиты

1.1. Генерация тестовой базы данных:

Создание структуры базы данных с таблицами: валюты, курсы валют, транзакции.

Возможность задать количество записей в каждой таблице.

Автоматическая генерация данных с случайными, но реалистичными значениями.

1.2. Работа с валютами:

Добавление, удаление и редактирование записей в таблице валют.

Поля таблицы: ID, название валюты, код валюты (ISO 4217), символ валюты.

1.3. Генерация курсов валют:

Автоматическое создание записей с курсами валют на определённую дату.

Поля таблицы: ID, дата, код валюты, курс относительно базовой валюты (например, USD).

Поддержка обновления данных через API.

1.4. Конвертер валют:

Выбор исходной и целевой валюты из списка.

Ввод суммы и вычисление конвертированной суммы на основании актуального курса валют.

Вывод истории конверсий.


2. Дополнительные функции

2.1. Экспорт данных:

Возможность экспорта данных из базы в форматe JSON.

Настройка полей для экспорта.

2.2. Импорт данных:

Импорт данных в таблицы валют и курсов валют.

2.3. Валидация данных:

Проверка корректности введённых данных (например, проверка кода валюты по ISO 4217).

Обработка ошибок при генерации и импорте данных.

3. Требования к базе данных

3.1. Структура базы данных:

Таблица Currencies: ID, Name, Code, Symbol.

Таблица ExchangeRates: ID, Date, CurrencyCode, Rate.

Таблица Transactions: ID, Date, Amount, SourceCurrency, TargetCurrency, ConvertedAmount.

3.2. Производительность:

Оптимизация запросов к базе данных.

Индексация ключевых полей.
