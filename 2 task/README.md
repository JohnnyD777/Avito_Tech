# Avito_Tech
Internship
# Avito_Tech
Internship

Инструкция для получения скриншотов в папке output.

1. Скачать Python с официального сайта https://www.python.org/downloads/
2. Открыть командную строку Python. Для этого на ПК или ноутбуке открыть Пуск-> Поиск-> ввести python->
в диалоговом окне появится программа Python с номером текущей версии-> Кликнуть на нее для запуска

3. Для автоматизации тест-кейсов, написанных в программе TestRail, используется связка
 Python + pytest + Playwright. Для ее реализации следует выполнить следующие шаги:

- Установить зависимости: для этого в командной строке Python ввести следующую команду
  pip install playwright

- Установить браузеры: для этого в командной строке Python ввести следующую команду
  python -m playwright install

- Создать тестовый проект и настроить окружение: для этого в командной строке Python ввести следующий код

  from playwright.sync_api import Pag

 class LoginPage:
 def __init__(self, page):
 self.page = page

 def enter_username(self, username):
 self.page.fill('input[name="username"]', username)

 def enter_password(self, password):
 self.page.fill('input[name="password"]', password)

 def click_login_button(self):
 self.page.click('button[type="submit"]')

 def is_error_message_displayed(self):
 return self.page.is_visible('.error-message')
 
4. Создать фикстуру pytest в отдельном файле conftest.py (Фикстура в тестировании — это данные, которые используются
 в тестах для проверки корректности работы программного обеспечения. Они представляют собой набор значений, которые
 определяют состояние системы перед выполнением теста. Фикстуры позволяют изолировать тесты от внешних факторов и
 обеспечить их воспроизводимость)
 
 Для этого в командной строке Python ввести следующую команду
 
 import pytest
 from playwright.sync_api import sync_playwright

 @pytest.fixture(scope='class')
 def browser():
 with sync_playwright() as playwright:
 browser = playwright.chromium.launch(channel="chrome", headless=False)
 context = browser.new_context(ignore_https_errors=True)
 page = context.new_page()
 yield page
 page.close()
 browser.close()
 
5. Запустить тесты с помощью pytest: для этого в командной строке Python ввести следующую команду
pytest my_tests.py

6. Для того, чтобы сделать скриншот счетчиков с сайта Авито, необходимо:

- установить библиотеку в командной строке python, с помощью команды

   pip install pyautogui
 
- в командной строке Python ввести следующий код

 import os
 import pyautogui

 output_dir = 'output'
 if not os.path.exists(output_dir):
 os.makedirs(output_dir)

 # Захват скриншота
 im = pyautogui.screenshot()

 # Сохранение скриншота в папку output
 os.chdir(output_dir)
 im.save('screenshot.png')

 Этот код использует библиотеку pyautogui для захвата скриншота и модуль os для
 сохранения скриншота в папку output.
