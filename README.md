# BlankProject

## Сценарии автоматизации

**Переход на страницу**
- Меню "каталог курсов" (клик)
- Программирование (выделить)
- Тестировщик ПО (клик)

Итог: Вы на странице курса "Тестировщик ПО"

**Успешная регистрация**
- Поле "Имя" (сгенерировать ник, свыше 1 символа)
- "Номер" (сгенерировать номер)
- "Почта" (ваша почта или сгенерировать почту)
- Кнопка "Записаться" (клик)

Итог: Вы успешно зарегистрированы!

**Неуспешная регистрация**
- Поле "Имя"  (Ввести любой некорректный ник (цифры, символы и т.д.))
- "Номер"  (Ввести любой некорректный номер)
- "Почта" (Ввести любой некорректную почту)
- Кнопка "Записаться" (клик)

Итог: Вы не зарегистрированы

**Граничные значения (поле имя) (один символ)**
- Поле "Имя" (ввести 1 букву)
- ниже поля должен отобразиться текст "Должно быть не короче 2 символов"
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Форма пройти не должна

**Граничные значения (поле "Имя") (два символа)**
- Поле "Имя" (ввести 2 буквы (не символы, цифры))
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Вы зарегистрированы!

**Граничные значения (поле "Имя") (три символа)**
- Поле "Имя" (ввести 3 буквы (не символы, цифры))
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Вы зарегистрированы!

**Символы (поле "Имя")**
- Поле "Имя" (ввести любой символ (кроме дефиса))
- ниже поля должен отобразиться текст "Должно состоять из букв"
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Форма пройти не должна

**Цифры (поле "Имя")**
- Поле "Имя" (удалить символ и ввести любую цифру)
- ниже поля должен отобразиться текст "Должно состоять из букв"
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Форма пройти не должна

**Формат номера**
- Поле "Номер" (ввести любые буквы, символы)
- ниже поля должен отобразиться текст  "Номер в формате +9 (999) 999-99-99"
- Ввести корректные данные для всех остальных полей и нажать на "Записаться"

Итог: Форма пройти не должна

**Пустые поля**
- Кнопка "Записаться" (клик)
- ниже всех полей должна появиться надпись "Обязательное поле"

Итог: Вы не зарегистрированы!

**Применение промокода**
- Кнопка "У меня есть промокод" (клик)
- Поле "Промокод" (ввести корректный код)
- Кнопка "Применить" (нажать)

Итог: Числовое значение стоимости курса должно снизиться

**Неуспешное примение промокода**
- Кнопка "У меня есть промокод" (клик)
- Поле "Промокод" (ввести некорректный код)
- Кнопка "Применить" (нажать)

Итог: Ниже должна появиться надпись "Неверный промокод"

**Состояние регистрации**
- Кнопка "Войти" (клик)
- Заполнить логин и войти в существующий аккаунт
- Выше должно появится окошко "Вы вошли %ваш_логин%"

Итог: Поля e.mail быть не должно (проверить наличие поля)

**Дата проведения курса**
- Выше формы регистрации есть надпись "Стартует через % дней" (выделить блок и проверить)

Итог: Вместо % должна быть разница между датой текущей и датой ближайшего курса "Тестировщик ПО"

**Стоимость курса**
- Цена стоимости курса  (выделить блок и проверить соотвествие с бд)
- Цена стоимости курса без скидки (выделить блок и проверить соотвествие с бд)
- Цена стоимости скидки  (выделить блок и проверить соотвествие с бд)
- Цена оплаты по месяцам (выделить блок и проверить соотвествие с бд)

Итог: Все должно соответствовать с данными бекэнда

**Получить консультацию**
- Кнопка "Получить консультацию" (клик)

Итог: ?Должно появится окошко с чатом конультанта?

**Политика**
- Кнопка "политики"

Итог: Вы должны перейти на страницу "ПОЛИТИКА ОБРАБОТКИ ПЕРСОНАЛЬНЫХ ДАННЫХ ПОЛЬЗОВАТЕЛЕЙ САЙТА"

**Соглашения**
- Кнопка "пользовательского соглашения" (клик)

Итог: Вы должны перейти на страницу "Пользовательское соглашение"

**Статья**
- Кнопка "статье" (клик)

Итог: Вы должны перейти на страницу "Как получить налоговый вычет за обучение: на что обратить внимание и стоит ли оформлять его через посредников"

-----------------------------------------------------------------------------------------------------------------

## Инструменты

Работа будет выполнятся в IntelliJ Idea. Его интефейс может облегчить процесс и даже ускорить его.
Из его плагинов будут применяться...

Java 11 - потому-что других ПОКА не знаю, ну и потому-что на нём очень много всего написано

Maven - удобное средство сборки проекта

Jacoco - для отчётов

Faker - для генерации ников и номеров

JUnit Jupiter - для тестов

Selenide - для работы и тестирования проекта в веб

%система_бд% нетологии - для работы с базой данных


## Разрешения, данные и доступ

Для данного проекта тестирования необходимы будут следующие разрешения...
- Разрешение на тестирование сайта
- Доступ к базе данных
- Доступ к API
- 1 зарегистрированный пользователь
- 1 телефон

## Возможные риски

Возможны небольшие трудности с тестированием цен (их может быть сложно будет выделить). Даты дают некоторую неопределённость.

## Необходимые специалисты

Для тестирования этой формы потребуется:
- 1 QA-тестировщик (ручной, либо автоматизатор).
- (возможно некоторое привлечение некоторых членов команды для уточнения вопросов)

## Оценка с учетом рисков в часах

Оценка времени: 3 часа
