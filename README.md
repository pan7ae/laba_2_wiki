# Теория 6 рукопожатий на Wikipedia



## Часть 1: Краткая устная реализация задачи, план, и технологии

Задача заключается в написании приложения на языке Python, которое будет анализировать ссылки на Википедии и находить цепочку переходов между двумя заданными страницами.

### План:
* Получить входные данные - два URL и ограничение на количество запросов в минуту;
* Написать функцию для получения страницы Википедии и извлечения всех ссылок на другие страницы; * Википедии из основного блока статьи и блока "References";
* Реализовать алгоритм поиска в ширину (BFS) для нахождения кратчайшего пути между двумя страницами Википедии, с учетом ограничения на количество запросов в минуту;
* Если кратчайший путь не найден за 5 шагов, сообщить об этом;
* Если путь найден, вывести его.

Технологии:
* Библиотека `requests` для выполнения HTTP-запросов к Википедии;
* Библиотека `BeautifulSoup` для парсинга HTML-страниц и извлечения ссылок;
* Библиотека `typing` для аннотации типов;
* Встроенные библиотеки Python, такие как `time` для управления скоростью запросов и `collections` для реализации алгоритма BFS.

Выбор именно этих технологий обосновывается их широкой распространенностью, хорошей документацией и простотой использования. В качестве альтернатив можно рассмотреть использование библиотек scrapy или aiohttp для асинхронных запросов, однако они более сложны в использовании и могут быть избыточны для данной задачи.
