# Kokoa Clone Update

HTML and CSS are so much fun!

### #1.3 Software Requirements

1. 구글 크롬 or 브레이브
2. visual studio code
3. github desktop

### #2.1 Setup and Errors

Community Material Theme  
Material Icon Theme

### #2.2 Our First HTML Tag

prettier - settings

- editor: Format On Save 체크
- editor : Default Formatter ‘esbenp.prettier-vscode 선택

h1 ~ h6

### #2.3 More Tags and Prettier

ul, ol - li

### #2.4 Tag Attributes

a : href, target(\_blank)  
img : src

### #2.5 More Tags and Head

head - title

### #2.6 Its All About the Head

meta : charset(utf-8), name(description) - content  
link : rel(shortcut icon), href

### #2.7 More Tags

- html tags mdn

p - abbr : title, mark, strong, sup, sub  
pre  
cite  
code  
audio : controls, autoplay, src  
dialog : open

### #2.8 Form Tags

form - input : type(file, text, password, submit), accept(image/\*, .pdf), required, placeholder, minlength, value

### #2.9 More Tags and IDs

label : for  
input : id, type(date)

### #2.10 Semantic HTML

header  
main - span, address  
footer

### #3.0 How to Add CSS to HTML

link : rel(stylesheet), href  
style

### #3.1 Writing Our First CSS Lines

tag {}  
color, text-decoration, font-weight, font-style, font-size, text-align

### #3.3 Blocks and Inlines

height, width, background-color

### #3.4 Margin Part One

margin, margin-top, margin-left, margin-right, margin-bottom

### #3.6 Paddings and IDs

padding

### #3.7 Border

\* {}, #id {}  
border

### #3.8 Classes

.class{}  
border-radius

### #3.9 Inline Block

display

### #3.10 Flexbox Part One

display: flex;  
justify-content, align-items

### #3.11 Flexbox Part Two

flex-direction, flex-wrap

### #3.12 Fixed

position: fixed;  
top, left, bottom, right  
opacity

### #3.13 Relative Absolute

```CSS
parent {
  position: relative;
}
child {
  position: absolute;
}
```

### #3.14 Pseudo Selectors part One

:first-child, :last-child, :nth-child(n, 2n, 2n+1, even, odd)

### #3.15 Combinators

parent child {}  
parent > child {}  
sibling + sibling {}

### #3.16 Pseudo Selectors part Two

sibling ~ sibling {}  
tag:attribute {}  
tag[attrigute="value"] {}  
tag[attribute-="word"] {}

### #3.17 States

:active, :hover, :focus  
a:visited {}  
form:focus-within {}  
form:hover input:focus {}

### #3.18 Recap

::selection, ::first-letter, ::first-line

### #3.19 Colors and Variables

```CSS
:root {
  --main-color: #489ee3;
  --default-border: 1px solid var(--main-color);
}

a {
  color: var(--main-color);
  border: var(--default-border);
}
```

### #4.0 Transitions

text-decoration  
transition: all 1s ease-in-out;

### #4.2 Transformations

transform: rotate, scale, translate, skew, matrix  
transition: transform 2s ease-in-out;

cubic-bezier: <https://matthewlein.com/tools/ceaser>

### #4.3 Animations part One

```CSS
@keyframes superSexyCoinFlip {
    form {
        transform: rotateY(0);
    }
    to {
        transform: rotateY(100deg) translateX(100px);
    }
}

img:hover {
    animation: superSexyCoinFlip 5s ease-in-out infinite;
}
```

### #4.4 Animations part Two

```CSS
@keyframes superSexyCoinFlip {
    0% {
        transform: rotateY(0);
    }
    25% {
        transform: scale(2);
    }
    50% {
        border-radius: 0px;
        transform: rotateY(180deg) translateY(-100px);
        border-color: tomato;
        opacity: 0;
    }
    75% {
        transform: scale(5);
        border-radius: 20px;
    }
    100% {
        transform: rotateY(0) translateY(0px);
    }
}
```

animista: <https://animista.net>

### #4.5 Media Queries

```CSS
@media screen and (min-width: 601px) and (max-width: 1200px) and (orientation: portrait) {
    div {
        background-color: wheat;
    }
}
@media screen and (orientation: landscape) {
    span {
        display: none;
    }
}
```

### #4.6 Media Queries Recap

CSS media query MDN

```CSS
@media screen and (min-device-width: 601px) and (max-width: 1200px) and (orientation: portrait) {
    div {
        background-color: wheat;
    }
}
@media print {
    div {
        background-color: tomato;
    }
}
```

### #5.0 What is Git

git: <https://git-scm.com>  
github: <https://github.com>

### #6.0 Introduction

.gitignore

### #6.2 BEM

BEM(Block Element Modifier)

```CSS
.btn {} //블록
.btn__price {} //price라는 정보
.btn--orange {} //modifier
.btn--big {} //modifier
```

```HTML
<a class="btn btn--big btn--orange" href="https://css-tricks.com">
    <span class="btn__price">$9.99</span>
    <span class="btn__text">Subscribe</span>
</a>
```

### #6.3 Font Awesome

Heroicons : <https://heroicons.dev>
Fontawesome : <https://fontawesome.com>

### #6.5 Status Bar CSS

Google Fonts : <https://fonts.google.com>

```css
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap");
body {
  font-family: "Open Sans", sans-serif;
}
```

```css
.status-bar {
  display: flex;
  justify-content: center;
}
.status-bar__column {
  width: 33%;
}
.status-bar__column:nth-child(2) {
  display: flex;
  justify-content: center;
}
.status-bar__column:last-child {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
```

### #6.6 Sign Up Screen part Three

reset CSS : <https://cssdeck.com/blog/scripts/eric-meyer-reset-css>

```css
@import "reset.css";
@import "status-bar.css";
```

### #6.7 Log In Form part One

resetCSS

```css
input:focus {
  outline: none;
}
```

variables.css

```css
:root {
  --yellow: #fae100;
}
```

Login Form

```css
#login-form input {
  border: none;
  padding: 15px 0px;
  font-size: 18px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
  margin-bottom: 25px;
  transition: border-color 0.3s ease-in-out;
}
#login-form input::placeholder {
  color: rgba(0, 0, 0, 0.4);
}
#login-form input:focus {
  border-color: var(--yellow);
}
```

### #6.8 Log In Form part Two

```css
button {
  cursor: pointer;
  cursor: not-allowed;
  cursor: progress;

  padding: 20px 0px;
  border-radius: 5px;
}

a {
  text-decoration: none;
  color: inherit;
}
```

### #6.9 Recap and Forms

### #6.10 Navigation Bar part One

### #6.11 Navigation Bar part Two

### #6.12 Border Box

### #6.13 Navigation Bar part Three
