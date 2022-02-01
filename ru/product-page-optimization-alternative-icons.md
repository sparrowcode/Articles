С помощью  [Product Page Optimization](https://developer.apple.com/app-store/product-page-optimization/) вы можете создавать варианты скриншотов, промо-текстов и иконок. Скриншоты и текст добавляются в App Store Connect, а вот иконки добавляет разработчик в Xcode-проект.

В документации сказано «поместите иконки в Asset Catalog, отправьте бинарный файл в App Store Connect и используйте SDK». Но как закинуть иконки и что за SDK - не сказали. Давайте разбираться, шаги подкрепил скриншотами.

## Добавляем иконки в Assets

Алтернативную иконку делаем в нескольких разрешениях, как и основную. Я использую приложение [AppIconBuilder](https://apps.apple.com/app/id1294179975). Неймнг пишем любой, но учтите - имя отобразится в App Store Connect.

![Добавляем иконки в Assets](https://cdn.ivanvorobei.by/websites/sparrowcode.io/product-page-optimization-alternative-icons/adding-icons-to-assets.png)

## Настройки в таргете

Нужен Xcode 13 и выше. Выберите таргет приложения и перейдите на вкладку `Build Settings`. В поиск вставьте `App Icon` и вы увидите секцию `Asset Catalog Compiler`.

![Настройки в таргете](https://cdn.ivanvorobei.by/websites/sparrowcode.io/product-page-optimization-alternative-icons/adding-settings-to-target.png)

Нас интересуют 3 параметра:

`Alternate App Icons Sets` - перечисление названий иконок, которые добавили в каталог.

`Include All App Icon Assets` - установите в `true`, что бы включить альтернативные иконки в сборку.

`Primary App Icon Set Name` - название иконки по умолчанию. Не проверял, но скорее всего альтернативную иконку можно сделать основной.

## Cборка

Остается собрать приложение и отправить на проверку.

***Альтернативные иконки будут доступны после прохождения ревью.***

Теперь можно собирать разные страницы приложения и создавать ссылки для A/B тестов.

