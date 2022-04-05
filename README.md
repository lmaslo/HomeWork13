# Проект по автоматизации тестирования для wildberries
<a target="_blank" href="https://www.wildberries.ru//">Веб сайт wildberries</a>

## :drop_of_blood: Содержание:

- [Реализованные проверки](#earth_africa-Реализованные-проверки)
- [Технологии](#earth_africa-Технологии)
- [Сборка в Jenkins](#earth_africa-Jenkins-job)
- [Запуск из терминала](#earth_africa-Запуск-тестов-из-терминала)
- [Allure отчет](#earth_africa-Allure-отчет)
- [Отчет в Telegram](#earth_africa-Уведомление-в-Telegram-при-помощи-бота)
- [Видео примеры прохождения тестов](#earth_africa-Примеры-видео-о-прохождении-тестов)


## :boom: Реализованные проверки

- ✓ Проверка логотипа
- ✓ Проверка функции поиска по тексту
- ✓ Проверка текста ошибки на странице авторизации/регистрации
- ✓ Проверка страницы Адреса
- ✓ Проверка ошибок в логах браузера


## :classical_building: Технологии

<p align="center">
<img width="6%" title="Idea" src="image/logo/Idea.svg">
<img width="6%" title="Java" src="image/logo/Java.svg">
<img width="6%" title="Selenide" src="image/logo/Selenide.svg">
<img width="6%" title="Selenoid" src="image/logo/Selenoid.svg">
<img width="6%" title="Allure Report" src="image/logo/Allure_Report.svg">
<img width="6%" title="Gradle" src="image/logo/Gradle.svg">
<img width="6%" title="JUnit5" src="image/logo/JUnit5.svg">
<img width="6%" title="GitHub" src="image/logo/GitHub.svg">
<img width="6%" title="Jenkins" src="image/logo/Jenkins.svg">
<img width="6%" title="Telegram" src="image/logo/Telegram.svg">
</p>


## <img src="images/logo/Jenkins.svg" width="25" height="25"  alt="Jenkins"/></a> Jenkins <a target="_blank" href="https://jenkins.autotests.cloud/job/10_DikayaAV_unit13/"> job </a>
<p align="center">
<a href="https://jenkins.autotests.cloud/job/10_DikayaAV_unit13/"><img src="images/screens/Screenshot_522.png" alt="Jenkins"/></a>
</p>

### :maple_leaf: Параметры сборки в Jenkins:

- browser (браузер, по умолчанию chrome)
- version (версия браузера, по умолчанию 91.0)
- size (размер окна браузера, по умолчанию 1920x1080)
- remoteUrl (логин, пароль и адрес удаленного сервера selenoid)

## :japanese_ogre: Запуск тестов из терминала

Локальный запуск:
```
gradle clean test
```

Удаленный запуск:
```
clean
test
-Dbrowser=${BROWSER}
-Dversion=${VERSION}
-Dsize=${BROWSER_SIZE}
-Durl=${REMOTE_URL}
```

## <img src="images/logo/Allure.svg" width="25" height="25"  alt="Allure"/></a> Отчет в <a target="_blank" href="https://jenkins.autotests.cloud/job/10_DikayaAV_unit13/allure/">Allure report</a>

### :lady_beetle: Основное окно

<p align="center">
<img title="Allure Overview Dashboard" src="images/screens/Screenshot_523.png">
</p>

### :cherries: Тесты

<p align="center">
<img title="Allure Tests" src="images/screens/Screenshot_524.png">
</p>

### :cut_of_meat: Графики

<p align="center">
<img title="Allure Graphics" src="images/screens/Screenshot_525.png">
</p>

## <img src="images/logo/Telegram.svg" width="25" height="25"  alt="Allure"/></a> Уведомление в Telegram при помощи бота

<p align="center">
<img title="Allure Overview Dashboard" src="images/screens/Screenshot_528.png" >
</p>

