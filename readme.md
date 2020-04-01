# Разбор структуры проекта простого Android-приложения

### Сборка проекта

Для сборки проекта используется [gradle](https://ru.wikipedia.org/wiki/Gradle).  
У нас есть 2 основных файла которые чаще всего приходится редактировать.
[build.gradle](build.gradle), лежащий в корне проекта и [app/build.gradle](app/build.gradle) из модуля app.
Самое простейшее для чего используются эти файлы - это для добавления зависимостей на библиотеки.
Например, для добавления зависимостей на [Timber](https://github.com/JakeWharton/timber) необходимо в [app/build.gradle](app/build.gradle)
в блок `dependencies` добавить строчку `implementation 'com.jakewharton.timber:timber:4.7.1'`

### Основные компоненты проекта

Код приложения лежит в [app/src/main](app/src/main/java)

Ресурсы приложения в [app/src/main/res](app/src/main/res)

К ресурсам относятся строки, размеры, цвета, лэйауты, картинки, стили.
Почитать подробнее можно [тут](https://developer.android.com/guide/topics/resources/providing-resources?hl=ru)

Манифест (файл, в котором необходимо прописывать все компоненты приложения, такие как Activity, Service итд) [app/src/main/AndroidManifest.xml](app/src/main/AndroidManifest.xml)
Подробнее [тут](https://developer.android.com/guide/topics/manifest/manifest-intro?hl=ru)