# План автоматизации тестирования сценария перехода к форме записи на обучение профессии «Тестировщик ПО» и заполнения этой формы.  

## 1. Перечень автоматизируемых сценариев.
**1. Сценарии навигации с главной страницы сайта Нетология.**

1)                 
- открыть в браузере главную страницу сайта Нетология https://netology.ru/  
- выбрать в разделе «Направления обучения» раздел «Программирование» 
- проскроллить страницу до профессии «Тестировщик ПО»
- выбрать блок «Тестировщик ПО». 

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

2) 
- открыть в браузере главную страницу сайта Нетология https://netology.ru/
- нажать в меню кнопку «Каталог курсов»  
- ввести в строку поиска «Какой курс вам нужен? » значение «Тестировщик ПО» 
- выбрать из выпадающего списка «Тестировщик ПО».

ОР - отображается страница с формой записи на курс «Тестировщик ПО». 

3) 
- открыть в браузере главную страницу сайта Нетология https://netology.ru/
- нажать в меню кнопку «Каталог курсов»  
- ввести в строку поиска «Какой курс вам нужен? » значение «Тестировщик ПО» 
- нажать «Enter».

ОР - отображается страница с формой записи на курс «Тестировщик ПО». 
              
4) 
- открыть в браузере главную страницу сайта Нетология https://netology.ru/
- нажать в меню кнопку «Каталог курсов»  
- ввести в строку поиска «Какой курс вам нужен? » значение «Тестировщик ПО»
- нажать «Найти курс».

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

5)
- открыть в браузере главную страницу сайта Нетология https://netology.ru/
- нажать в меню кнопку «Каталог курсов»  
- выбрать в выпадающем меню «Направления обучения» раздел «Программирование» 
- проскроллить страницу до профессии «Тестировщик ПО»
- выбрать блок «Тестировщик ПО». 

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

**Сценарии навигации со страницы профессии:**

1)
- открыть в браузере страницу профессии «Тестировщик ПО» https://netology.ru/programs/qa
- проскроллить страницу вниз до формы записи на курс.

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

2)
- открыть в браузере страницу профессии «Тестировщик ПО» https://netology.ru/programs/qa
- нажать в блоке описания кнопку «Записаться». 

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

3)
- открыть в браузере страницу профессии «Тестировщик ПО» https://netology.ru/programs/qa
- проскроллить страницу ниже до появления сверху всплывающего меню 
- нажать в всплывающем меню кнопку «Записаться».  

ОР - отображается страница с формой записи на курс «Тестировщик ПО».

**2. Сценарии заполнения и отправки формы записи на обучение профессии «Тестировщик ПО».**

Описание валидных данных:
1) валидными данными для поля «Имя» считаются имя на кириллице заглавными или строчными буквами, от 2 до 100 символов, например, Анна.
2) валидными данными для поля «Имя» считаются имя на латинице заглавными или строчными буквами,  от 2 до 100 символов, например, Sveta. 
3) валидными данными для поля «Имя» считается наличие пробела, например, Анна Мария.                 
4) валидными данными для поля «Имя» считается наличие «-», например, Анна-Мария. 
5) валидными данными для поля «Телефон» считаются  цифры. Номер в формате +9 (999) 999-99-99, без пробелов. Количество цифр 11, например, +79201345680.
6) валидными данными для поля «Электронная почта» считаются наличие знака @ и домена почтовых сервисов. Адрес может быть указан на кириллице или латинице заглавными или строчными буквами, от 2 до 100 символов. Например, example@example.ru. 

Позитивные сценарии:

1) 
- заполнить поля «Имя», «Телефон», «Электронная почта» валидными данными 
- нажать кнопку «Записаться».                                                                        

ОР - переход на страницу оплаты.

Негативные сценарии:

1) 
- оставить поле «Имя» незаполненным 
- заполнить поле «Телефон» валидными данными.
      
ОР - появляется ошибка «Обязательное поле». 

2)
- заполнить поле «Имя» невалидными данными - числовыми значениями, например, 5678. 

ОР - появляется ошибка «Должно состоять из букв». 
                                                                
3)
- заполнить поле «Имя» невалидными данными - 1 символом на кириллице, например, а.

ОР - появляется ошибка «Должно быть не короче 2 символов». 

4) 
- заполнить поле «Имя» валидными данными
- оставить поле «Телефон» незаполненным. 
     
ОР - появляется ошибка «Обязательное поле». 

5) 
- заполнить поле «Телефон» невалидными данными - символы на кириллице, например, привет. 

ОР - появляется ошибка «Номер в формате +9 (999) 999-99-99». 

6) 
- заполнить поле «Телефон» невалидными данными - номер короче 11 цифр, например,+7883. 

ОР - появляется ошибка «Номер в формате +9 (999) 999-99-99». 

7) 
- заполнить поля «Имя», «Телефон» валидными данными
- оставить поле «Электронная почта» незаполненным. 
                                    
ОР - появляется ошибка «Обязательное поле». 

8)
- заполнить поле «Электронная почта» невалидными данными - символы на латинице, без знака @, например, example.ru.

ОР - появляется ошибка «Неверный email».

9)
- заполнить поле «Электронная почта» невалидными данными - символы на латинице, без домена почтовых сервисов, например, example@example.

ОР - появляется ошибка «Неверный email».

**3. API тесты**

Позитивные сценарии:

1) проверка заявки на запись курса в базе данных. 
     
## 2. Перечень используемых инструментов с обоснованием выбора.

IntelliJ IDEA - среда разработки для Java. 

Junit5 - платформа дла написания автотестов и их запуска.

Java - язык написания автотестов.

Gradle - инструмент автоматизации сборки и управления зависимостями.

Git и GitHub - хранение кода, в том числе автотестов. 

Lombok - аннотация, которая позволяет генерировать код.

Selenide - фреймворк для автоматизированного тестирования веб-приложений. 

Docker - система контейнеризации.

Docker Compose для запуска мультиконтейнерных приложений.

JDBC для взаимодействия с SQL базами данных.  

Apache Commons DbUtils для упрощения работы с с JDBC. 

Allure - фреймворк для репортинга. 
                                                           
## 3. Перечень необходимых разрешений, данных и доступов.

Разрешение на автоматизированное тестирование владельца сайта.

Документация.

Запрос валидных данных для тестового пользователя.

Запрос доступа к БД, API. 

## 4. Перечень и описание возможных рисков при автоматизации.

Обнаружение неработающего функционала.

Изменение структуры страницы.

Отсутствие тестовых меток.

## 5. Перечень необходимых специалистов для автоматизации.

Специалист по автоматизированному тестированию.

## 6. Интервальная оценка с учётом рисков в часах.

Планирование автоматизации тестирования - 24 часа. 

Запуск приложения и настройка окружения - 24 часа.

Написание автотестов, тестирование и отладка - 336 часов.

Формирование и подготовка отчетов - 48 часов.
