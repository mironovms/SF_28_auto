Files
-----

[conftest.py](conftest.py) contains all the required code to catch failed test cases and make screenshot
of the page in case any test case will fail.

[pages/base.py](pages/base.py) contains PageObject pattern implementation for Python.

[pages/elements.py](pages/elements.py) contains helper class to define web elements on web pages.

[tests/test_auth_page.py](tests/test_auth_page.py) contains several tests for Rostelekom (https://b2c.passport.rt.ru/)


How To Run Tests
----------------

1) Install all requirements:

    ```bash
    pip3 install -r requirements.txt
    ```

2) Download Selenium WebDriver from https://chromedriver.chromium.org/downloads (choose version which is compatible with your browser)

3) Run tests:

    ```bash
    python3 -m pytest -v --driver Chrome --driver=Chrome --driver-path=/chromedriver tests/*
    ```


Note:
~/chrome in this example is the file of Selenium WebDriver downloaded and unarchived on step #2.