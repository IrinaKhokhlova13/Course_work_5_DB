# ** Курсовая работа. Работа с базами данных **
>###### main.py - файл запуска программы

🧑🏻‍💻 В рамках проекта вам необходимо получить данные о компаниях и вакансиях с сайта [hh.ru](hh.ru), спроектировать таблицы в БД PostgreSQL и загрузить полученные данные в созданные таблицы.

## Основные шаги проекта

  * Получить данные о работодателях и их вакансиях с сайта [hh.ru](hh.ru). Для этого используйте публичный API [hh.ru](hh.ru) и библиотеку ___requests___.
  * Выбрать не менее 10 интересных вам компаний, от которых вы будете получать данные о вакансиях по API.
  * Спроектировать таблицы в БД Postgres для хранения полученных данных о работодателях и их вакансиях. Для работы с БД используйте библиотеку ___psycopg2___.
  * Реализовать код, который заполняет созданные таблицы в БД Postgres данными о работодателях и их вакансиях.
  * Создать класс DBManager для работы с данными в БД.

## Класс DBManager

Создайте класс DBManager, который будет подключаться к БД Postgres и иметь следующие методы:

  * ___get_companies_and_vacancies_count()___: получает список всех компаний и количество вакансий у каждой компании.
  * ___get_all_vacancies()___: получает список всех вакансий с указанием названия компании, названия вакансии и зарплаты и ссылки на вакансию.
  * ___get_avg_salary()___: получает среднюю зарплату по вакансиям.
  * ___get_vacancies_with_higher_salary()___: получает список всех вакансий, у которых зарплата выше средней по всем вакансиям.
  * ___get_vacancies_with_keyword()___: получает список всех вакансий, в названии которых содержатся переданные в метод слова, например “python”.

Класс DBManager должен использовать библиотеку ___psycopg2___ для работы с БД.