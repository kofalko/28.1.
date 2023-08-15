# 28.1.Итоговый проект по автоматизации тестирования (PJ-04)
conftest.py содержит весь необходимый код для отлова неудачных тестовых случаев и создания скриншота страницы в случае, если какой-либо тестовый пример не сработает.

pages/base_page.py содержит реализацию шаблона PageObject для Python.

pages/auth_page.py страница авторизации для работы с автотестами.

pages/config_page.py страница регистрации для работы с автотестами.

pages/elements.py содержит вспомогательный класс для определения веб-элементов на веб-страницах.

tests_rostelecom.py содержит тесты для Ростелекома ( https://b2c.passport.rt.ru/ )

Запуск тестов

Установите все требования: pip install -r requirements.txt

Загрузите Selenium WebDriver с https://chromedriver.chromium.org/downloads (выберите версию, совместимую с вашим браузером)

Запустите тесты: pytest -v --driver Chrome --driver-path /chromedriver tests_rostelecom.py
