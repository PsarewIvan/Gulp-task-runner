# Gulp-сборщик.

Сборщик frontend-проектов

## Установка

```
$ npm init
```

## Использование

```
$ gulp dev
```
Запускает весь сборщик и создает локальный сервер с LiveReload


```
$ gulp devMin
```
Запускает сборщик без копирования и минификации всех изображений и svg. Создает локальный сервер с LiveReload


```
$ gulp build
```
Запускает весь сборщик без создания сервера.


```
$ gulp buildWithoutImg
```
Запускает сборщик без копирования и минификации всех изображений, svg и без создания сервера.


```
$ gulp buildImg
```
Запускает оптимизацию и минификацию изображений, создает svg-спрайт.

### Перечень всех тасков (не описанных выше)

- gulp html
- gulp styles
- gulp scripts
- gulp fonts
- gulp img
- gulp webp
- gulp svg
- gulp svgSprite
- gulp cleanWithoutImg
- gulp cleanImg
- gulp cleanAll
- gulp watch

### Структура src

```
src
  fonts
    **/*.[woff, woff2]
  html
    index.html
    *.html
  img
    icon
      **/*.svg
    picture
      **/*.[jpg, png]
    svgSprite
      **/*.svg
  js
    library
      **/*.js
    scripts
      **/*.
    main.js
  scss
    blocks
      **/*.scss
    global
      fonts.scss
      normilize.scss
      scaffolding.scss
      var.scss
      **/*.scss
    main.scss

```

### Структура build

```
build
  css
    styles-min.css
  img
    icon
      **/*.svg
    picture
      **/*.[jpg, png]
    svgSprite
      sprite.svg
    webp
      **/*.webp
  fonts
    *.[woff, woff2]
  js
    script-min.js
  index.html
  *.html
```
