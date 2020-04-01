# Разбор структуры проекта простого Android-приложения

Для сборки проекта используется [gradle](https://ru.wikipedia.org/wiki/Gradle).  
У нас есть 2 основных файла которые чаще всего приходится редактировать.
[build.gradle](build.gradle), лежащий в корне проекта и [app/build.gradle](app/build.gradle) из модуля app.
Самое простейшее для чего используются эти файлы - это для добавления зависимостей на библиотеки.
Например, для добавления зависимостей на [Timber](https://github.com/JakeWharton/timber) необходимо в [app/build.gradle](app/build.gradle)
в блок `dependencies` добавить строчку `implementation 'com.jakewharton.timber:timber:4.7.1'`
