<h2 align="center">Universal private policy</h2>

<p>Универсальное сообщение о том, что на сайте имеется политика конфиденциальности</p> 

## Содержание

1. **[Install](#install)**
2. **[CSS](#css)**

---

## Install

<p>Подключаем файлы</p>

```html
<head>
    <!--CSS-->
    <!--
    * Выбераем один из перечисленных ниже css-пресетов, по умолчанию используется dark-bottom.css, в котором необходимо изменить цвет кнопки и\или ссылки в стиле сайта
    * Что бы не загрязнять код, лучше скопировать лишь нужный CSS без комментариев.
    * Скриншоты примеров можно найти в папке presets
    -->
    <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/dark-bottom.css" type="text/css"/>
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/dark-top.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/dark-floating.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/dark-floating-tada.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/dark-inline.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/light-bottom.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/light-top.css" type="text/css"/>-->
    <!--<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/light-floating.css" type="text/css"/>-->
    <!--/CSS-->

    <!--JS-->
    <!--
    * Подключаем javascript и настраиваем параметры ниже в зависимости от сайта, здесь все вроде элементарно и просто
    * На сайте должен быть подключен jQuery!
    -->
    <script type="text/javascript">
        window.cookieconsent_options = {
            message: 'Пользуясь сайтом https://arahort.pro/, Вы автоматически принимаете правила передачи и обработки персональных данных.',
            learnMore: 'Подробнее',
            link: '/policy/',
            target: '_blank',
            dismiss: 'Я согласен.',
            theme: 'dark-bottom'
        };
    </script>
    <script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/1.0.10/cookieconsent.min.js"></script>
    <!--/JS-->
</head>
```

---

## CSS

<p>Полоску можно сделать полупрозрачной, для этого если используется стандартная тема мы применяем стиль</p>

```css
.cc_container{background-color: rgba(0, 0, 0, 0.7) !important;}
```

<p>0.7 - степень прозрачности от 0 до 1</p>

<p>Если политику перекрывает JivoSite попробуйте:</p>

```css
.cc_container{z-index: 9999 !important;}
.jivo-iframe-container-bottom{z-index: 9000 !important;}
.jdiv{z-index: 9000 !important;}
.globalClass_ET{z-index: 9000 !important;}
._init_Tk{z-index: 9000 !important;}
```

---

## Автор

**[Alex Arahort](https://arahort.pro/)**

---

**[⬆ наверх](#Содержание)**

