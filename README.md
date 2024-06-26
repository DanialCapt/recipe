# Приложение "Рецептник"

Веб-приложение с базой данных рецептов.

Приложение написано на Flutter Dart.

Основной файл расположен в lib/main.dart

1. Приложение настроено на использование темной темы: theme: ThemeData.dark(),
2. Использовал асинхронные функции для получения данных из API с сайта https://developer.edamam.com/. Для этого я зарегистрировался на этом сайте, и использовал созданный ID и Key для ссылки.
getApiData() — функция, которая делает HTTP-запрос для получения данных рецептов в формате JSON и преобразует их в объекты класса Model.
Асинхронные запросы выполнены при помощи библиотеки http.
4. Система управления состоянием с помощью StatefulWidget
Два основных экрана (главная страница и страница поиска) управляются с помощью StatefulWidget.
Обновление состояния происходит через метод setState(), что обеспечивает автоматическое обновление пользовательского интерфейса при изменении данных.
5. Переходы между страницами и использование Navigator
Использование Navigator.push для перехода к новым экранам, например, к SearchPage или WebPage.
Обратная навигация осуществляется с помощью встроенной системы навигации Flutter.
6. Реализация поиска рецептов
Текстовое поле позволяет вводить поисковые запросы, передаваемые в API запрос.
SearchPage позволяет отображать результаты поиска рецептов на отдельном экране.
7. Отображение веб-страницы с рецептом
Экран WebPage содержит встроенный браузер WebView для отображения полной версии рецепта на внешнем сайте.
8. Структура данных с использованием класса Model
Класс Model обеспечивает удобную структуру для хранения данных о рецепте.

Это структурированный проект с использованием современных библиотек и методологий Flutter-разработки, который можно легко расширять для добавления новых функций и улучшения пользовательского опыта.
