# 1. C помощью BEM опишите человеческое тело

```
голова
    голова__глаза_зеленые
    голова__волосы_кудрявые
    голова__нос
тело
    тело__спина
    тело__пресс
    тело__шея
рука
    рука__локоть
    рука__кисть
    рука__пальцы_длинные
```

# 2. По варианту найти 4 различных блоков c точки зрения BEM: header, форма, карточка и один на выбор студента. Подготовить их создание в нотации Emmet с использованием BEM.

## 2.1. Header

<image src="/imgs/header.jpg" alt="Header view">

### Emmet:

```
header.header>a.header__logo[href="./index.html"]+nav.nav>a.nav__link[href="#"]*5+a.nav__link[href="/form.html"]+button.nav__button{"book a demo"}
```

### Result:

```
<header class="header">
    <a href="./index.html" class="header__logo"></a>
    <nav class="nav">
        <a href="#" class="nav__link"></a>
        <a href="#" class="nav__link"></a>
        <a href="#" class="nav__link"></a>
        <a href="#" class="nav__link"></a>
        <a href="#" class="nav__link"></a>
        <a href="/form.html" class="nav__link"></a><button class="nav__button">"book a demo"</button></nav>
</header>
```
## 2.2. Form

<image src="/imgs/form.jpg" alt="Form view">

### Emmet:

```
form.form>input.form__input.form__input_name+input.form__input.form__input_email+(div.form__double-input>input.form__input.form__input_company+input.form__input.form__input_position)+textarea.form__input.form__input_message.form__input_textarea+button.form__button.form__button_submit
```

### Result:

```
<form action="" class="form">
    <input type="text" class="form__input form__input_name">
    <input type="text" class="form__input form__input_email">
    <div class="form__double-input">
        <input type="text" class="form__input form__input_company">
        <input type="text" class="form__input form__input_position">
    </div>
    <textarea name="" id="" cols="30" rows="10" class="form__input form__input_message form__input_textarea"></textarea>
    <button class="form__button form__button_submit"></button>
</form>
```
## 2.3. Card

<image src="/imgs/card.jpg" alt="Card view">

### Emmet:

```
ul.post-cards>li.post-card>img.post-card__image+.post-card__desc>p.post-card__title+p.post-card__date
```

### Result:

```
<ul class="post-cards">
    <li class="post-card">
        <img src="" alt="" class="post-card__image">
        <div class="post-card__desc">
            <p class="post-card__title"></p>
            <p class="post-card__date"></p>
        </div>
    </li>
</ul>
```
## 2.4. Partners

<image src="/imgs/partners.jpg" alt="Partners view">

### Emmet:

```
div.partners>p.partners__title+div.partners__logos>img.partner__logo*6
```

### Result:

```
<div class="partners">
    <p class="partners__title"></p>
    <div class="partners__logos">
        <img src="" alt="" class="partner__logo">
        <img src="" alt="" class="partner__logo">
        <img src="" alt="" class="partner__logo">
        <img src="" alt="" class="partner__logo">
        <img src="" alt="" class="partner__logo">
        <img src="" alt="" class="partner__logo">
    </div>
</div>
```