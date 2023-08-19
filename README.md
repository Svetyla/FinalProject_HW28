# Финальный проект Skillfactory курса INTQAP

Автоматизированное UI-тестирование новой внешней авторизации в личном кабинете от заказчика Ростелеком Информационные Технологии ( https://b2c.passport.rt.ru/ )


-Сформированы тест-кейсы и отчёты о дефектах: [здесь](https://docs.google.com/spreadsheets/d/1sUnpUdUBwAnR7G65z6jEsN0BabYi27Zm8bdstazBmyc/edit?usp=sharing)

**1.** В папке pages в файле base_page.py находится конструктор webdriver и общие методы для всех тестируемых страниц.

**2.** В папке pages в файлах auth_page.py, change_pass_page.py, reg_page.py находятся методы проверок: 

файл auth_page.py содержит проверки методов авторизации;

файл change_pass_page.py содержит методы проверки формы восстановления пароля;

файл reg_page.py содержит методы проверки формы регистрации.

**3.** В папке с тестами в файлах test_auth_page.py, test_change_pass_page.py, test_reg_page.py находятся тесты.

Все тесты помечены номером, совпадающим с номером тест-кейса в файле: [здесь](https://docs.google.com/spreadsheets/d/1sUnpUdUBwAnR7G65z6jEsN0BabYi27Zm8bdstazBmyc/edit?usp=sharing)

Во всех файлах с тестами, имеются закомментированные команды для запуска тестов из командной строки.

запуск тестов формы авторизации: # python -m pytest -v --tb=linetests/test_auth_page.py;

запуск тестов формы восстановления восстановления: # python -m pytest -v --tb=линейные тесты/ test_change_pass_page.py;

запуск тестов формы регистрации: # python -m pytest -v --tb=линейные тесты/ test_reg_page.py)

**4.** В папке pages в файле "locators.py доступны все локаторы.

**5.** В корневой директории проекта: 

conftest.py - находится фиксура с открытием и закрытием браузера.

settings.py - хранятся методы и переменные для параметризации тестов.

pytest.ini - зарегистрированы метки маркировки тестов.

requirements.py - используются библиотеки.
