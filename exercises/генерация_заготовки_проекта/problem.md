## Генерация заготовки проекта

У вас должен быть установлен и настроен генератор `Yeoman` и `generator-bem-stub`.
Теперь в корневой папке `do-it-yourself-workshop` необходимо запустить команду:

```bash
yo bem-stub
```

Пройдемся по вопросам:

* “How to name the project?” («Как назвать проект?») — Имя проекта должно быть `bfs-stub`. Если оно будет отличаться от данного, то в дальнейшем могут быть проблемы с проверкой заданий.
* “Who will mantain this project?” («Кто будет вести проект?») — Нужно ввести свое имя или согласиться с предложенным.
* “What email to use?” («Какую почту использовать?») — Нужно ввести свой адрес электронной почты или согласиться с предложенным.
* “What collector to use?” («Какой сборщик использовать?») — мы используем инструмент `bem-tools`. Это утилита, которая будет собирать наш проект — склеивать стили, скрипты, шаблоны, компилировать и оптимизировать в соответствии с декларацией страницы, зависимостями блоков и файлами конфигурации.
* “What base library to use?” («Какую базовую библиотеку использовать?») – мы выбираем библиотеку [bem-core](http://ru.bem.info/libs/bem-core/), которая содержит в себе все необходимые нам технологии, шаблонизаторы и фреймворк для написания клиентского JavaScript — `i-bem.js`.
* “Would you like any additional libraries?” («Хотим ли мы использовать дополнительные библиотеки?») – в нашем проекте мы будем использовать библиотеку блоков [bem-components](http://ru.bem.info/libs/bem-components/). В ней есть опциональные стилевые темы.
* “What platforms to use?” («Какие уровни переопределения будем использовать?») - на нашем проекте мы будем использовать только уровень `desktop`. Остальные уровни нам не пригодятся.
* “Use design from bem-components?” («Использовать ли дизайн из библиотеки bem-components?») - в библиотеке bem-components для блоков реализовано несколько стиливых тем (реализация блоков в технологии CSS). В нешем проекте мы будем их использовать.
* “What technologies to use?” («Какие технологии использовать?») - мы будем использовать технологии `bemjson.js` для описания нашего БЭМ-дерева, `browser.js+bemhtml` для написание клиенсткого JS и `bemhtml` для шаблонизации. Т.е. вы должны выбрать 3 технологии - bemjson.js, browser.js+bemhtml и bemhtml.
* “Build static HTML?” («Генерировать ли HTML?») - Собственно, генерировать ли статичный HTML. Нам нужно выбрать `yes`.

После того, как вы сгенерируете заготовку проекта и установщик создаст все необходимые зависимости, нужно будет запустить проверку этого шага:
`node bfs-workshop.js verify`
