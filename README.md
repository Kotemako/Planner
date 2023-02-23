План автоматизированного тестирования формы заявки записи на курсы на сайте “Нетология”.

Перечень автоматизируемых сценариев.

Первый:
1. На главной странице выбрать “Каталог курсов”
2. В окне нужно выбрать “Программирование”
3. Далее на открывшейся странице со списком курсов выбрать “Тестировщик ПО”

Второй:
1. На главной странице в разделе “Направления обучения” выбрать “Программирование”
2. Далее как и в третьем пункете выше.

Третий:
1. Вариант через строку поиска - после клика на “каталог курсов” в строке поиска набрать начальные буквы “тестиров”
2. В результате поиска выбрать “Тестировщик ПО”
3. После попадания на страницу профессии “Тестировщик ПО” для перехода к форме записи необходимо промотать страницу вниз до конца или в начале страницы кликнуть по кнопке “Записаться”.

Сценарии тестирования формы записи.
Форма записи состоит из трех полей “Имя”, “Номер телефона”, “Электронная почта” и двух кнопок “Записаться” и “Получить консультацию”, а также двух ссылок на информацию с условиями пользовательского соглашения и политики сайта.

Сценарии тестирования самой формы записи можно разделить на две основные ветки: для зарегистрированных и незарегистрированных пользователей.

Для зарегистрированных пользователей поля формы записи заполняются автоматически данными из личного кабинета (ЛК) пользователя. 
В этом тест кейсе проверяем:
соответствие данных (автоматически заполненных полей формы) и данных из ЛК пользователя.
отправку формы.
в зависимости от требований, проверка возможности изменять данные на отличные от данных в ЛК.

Для незарегистрированных пользователей.
Ввод валидных значений во всех трех полях. Отправка формы. Варианты: по кнопке “записаться”, по кнопке “получить консультацию”.
Ввод невалидного имени. Проверка на всплывающее предупреждение. Варианты: имя через дефис, с “ё”, латиница, раздельное написание.
Ввод невалидного номера телефона. Проверка на всплывающее предупреждение. Варианты: без “+”, 1 цифра, больше 11.
Ввод невалидного email. Проверка на всплывающее предупреждение. Варианты: без “@”, без “.”, кириллица.
Отправка пустой анкеты. Проверка наличия предупреждающих сообщений под полями о необходимости их заполнения
Проверка перехода по ссылкам “пользовательские соглашения”, “политика”.

Перечень используемых инструментов
1. JDK 11. Код тестов на Java.
2. IntelliJ IDEA. Среда подготовки авто-тестов.
3. Github. Как репозиторий для хранения кода.
4. JUnit Jupiter. Фреймворк для тестирования.
5. Gradle. Система сборки кода.
6. Faker. Плагин для генерации данных.
7. Lombok. Плагин для минимизации строк кода за счет аннотаций.
8. Selenide. Продвинутый плагин для тестирования веб-интерфейса.

Перечень необходимых разрешений/данных/доступов
1. Зарегистрированный пользователь (данные для входа в ЛК) на портале netology.ru с заполненным профилем(имя, телефон, электронная почта)
2. Требования к полям формы: валидные варианты заполнения каждого поля.
3. Возможность отправки более одного раза формы с идентичными данными
4. Перечень и описание возможных рисков при автоматизации
5. Наличие точной и полной спецификации с требованиями к полям формы и структуре сайта в целом.
6. Изменение структуры и верстки страниц перехода к форме записи, а также ее полей. При даже незначительных изменениях возможно падение тестов и дальнейшая доработка .

Перечень необходимых специалистов для автоматизации
Инженер по тестированию.
Разработчик

Интервальная оценка с учётом рисков (в часах)
Ориентировочно оценка внедрения автоматизации в части формы записи - 70 часов.