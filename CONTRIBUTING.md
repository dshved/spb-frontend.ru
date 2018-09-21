# Contributing to spb-frontend.ru

## Gatsby

Сайт работает на движке [Gatsby](https://www.gatsbyjs.org/)
с несколькими дополнениями

- [gatsby-plugin-manifest](https://www.npmjs.com/package/gatsby-plugin-manifest)
- [gatsby-plugin-react-helmet](https://www.npmjs.com/package/gatsby-plugin-react-helmet)
- [gatsby-source-filesystem](https://www.npmjs.com/package/gatsby-source-filesystem)
- [gatsby-transformer-remark](https://www.npmjs.com/package/gatsby-transformer-remark)
- [plugin-feed](https://github.com/spb-frontend/spb-frontend.ru/tree/master/plugins/plugin-feed)

## Waffle.io [![Stories in Ready](https://badge.waffle.io/spb-frontend/spb-frontend.ru.svg?label=ready&title=Ready)](http://waffle.io/spb-frontend/spb-frontend.ru)

Мы ведем работу над сайтом в [waffle.io](http://waffle.io/spb-frontend/spb-frontend.ru)
В работе с waffle.io помогает [WaffleBot](https://help.waffle.io/wafflebot-basics/getting-started-with-the-wafflebot/how-to-use-the-wafflebot)

## Issues

Все созданные issues попадают в колонку _Backlog_,
когда задача готова к работе, она попадает в колонку _Ready_,
если берете задачу на себя, обязательно указывайте себя в _Assignees_
и двигайте задачу в колонку _In Progress_
или открывайте пулреквест в котором ссылайтесь на нужный issue, бот сам подвинет
задачу в In Progress, это необходимо, чтобы другие участники могли видеть,
кто над чем работает.

## Линтеры

### eslint

Мы используем eslint:recommended и plugin:react/recommended конфиги, но
переопределили некоторые правила.

Дополнительно используем плагины eslint-plugin-compat, eslint-plugin-import,
eslint-plugin-jsx-a11y, eslint-plugin-react

### stylelint

Для stylelint используем stylelint-config-standard c переопределенными
некоторыми правилами

### lint-staged

lint-staged перед коммитом проверяет файлы линтерами

- .js и jsx — с помощью eslint
- .css — с помощью stylelint

## Верстка

### компоненты

Все компоненты лежат в [/src/components](/src/components) у каждого компонента
должен быть index.js файл и опционально style.module.css, компонент не должен
использовать глобальные стили

### media queries

Размеры экранов на которые мы ориентируемся в верстке

- Мобильный — <= 480px
- Планшет — <= 1024px
- Десктоп — > 1024px

## PostCSS плагины

Мы пользуемся теми плагинами, которые поставляются вместе с Gatsby

## Браузеры

Мы не поддерживаем IE и ориентируемся на последние 2 версии остальных браузеров
и на браузеры используемые в мире больше чем 2% людей по статистике Can I Use
