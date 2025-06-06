# laba1web 

Генератор Резюме (Resume Builder)

Цей проєкт — це динамічний генератор резюме на JavaScript, який дозволяє користувачеві ввести особисту інформацію, освіту, досвід і навички, а потім згенерувати відформатоване резюме прямо на сторінці. Дані зберігаються у localStorage для подальшого редагування або повторного перегляду.

Основні функції

Створення резюме на основі введених даних.
Перевірка правильності заповнення полів (валідація).
Збереження інформації в localStorage.
Редагування збереженого резюме.
Очищення збережених даних.
Приклад структури коду з використанням класів, замикань та каррінгу.
Структура класів

PersonalInfo — зберігає ім’я, вік та контакти.
Education — містить опис освіти.
Experience — містить опис досвіду роботи.
Skills — обробляє список навичок.
Resume — головний клас, що об'єднує все та виводить HTML.
Як це працює

Користувач заповнює поля у HTML-формі.

Функція createResume() створює об'єкти, проводить валідацію та виводить HTML у DOM.

Дані зберігаються в браузері (localStorage).

Користувач може:

натиснути "Редагувати" — і дані підставляться назад у форму;
натиснути "Очистити" — і всі збережені дані видаляються.
Технології

JavaScript (ES6+)
localStorage
HTML (форма та блок виводу)
Об'єктно-орієнтований підхід
Замикання та каррінг
Приклад HTML-форми
<input id="name" placeholder="Ім’я">
<input id="age" placeholder="Вік">
<input id="contacts" placeholder="Контакти">
<input id="education" placeholder="Освіта">
<input id="experience" placeholder="Досвід">
<input id="skills" placeholder="Навички через кому">
<button onclick="createResume()">Створити</button>
<button onclick="editResume()">Редагувати</button>
<button onclick="clearStorage()">Очистити</button>
<div id="resumeDisplay"></div>
Запуск

Створити HTML-сторінку з формою (див. приклад вище).
Підключити до неї JavaScript-файл зі скриптом.
Відкрити сторінку у браузері та заповнити форму для створення резюме.
