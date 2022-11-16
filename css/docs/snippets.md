# Сниппеты и Триксы

### Применение `:root` для шрифтов

```css
:root {
  font-size: calc(1vw + 1vh + 0.5vmin);
}
```

### Вывод на экран атрибутов тега

```css
.icon:after {
  content: attr(aria-label);
}
```

### Лоботомированная сова

Все компоненты в структуре документа, получают margin-top: 1.5em.

```css
* + * {
  margin-top: 1.5em;
}
```

### Непрерывный вертикальный ритм

Непрерывный вертикальный ритм дополняет визуальной эстетикой, за счет этого чтение текста намного приятней.

```css
.intro > * {
  margin-bottom: 1.25rem;
}
```

### Блок с собственным отношением сторон

Применение padding 20% устанавливает высоту параллелепипеда равной 20% от его ширины. Вне зависимости от ширины окна, дочерний DIV продолжит сохранение соотношение сторон (100% / 20% = 5:1).

```css
.container {
  height: 0;
  padding-bottom: 20%;
  position: relative;
}

.container div {
  border: 2px dashed #ddd;
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
```

### Стили для битых изображений

```css
img {
  display: block;
  font-family: Helvetica, Arial, sans-serif;
  font-weight: 300;
  height: auto;
  line-height: 2;
  position: relative;
  text-align: center;
  width: 100%;
}
```

Сейчас следует дополнить правилами псевдо-элементы для изображения сообщения пользователю и URL-ссылки битого изображения:

```css
img:before {
  content: "Упс, изображение ниже поломалось :(";
  display: block;
  margin-bottom: 10px;
}

img:after {
  content: "(url: " attr(src) ")";
  display: block;
  font-size: 12px;
}
```

### Оптимизация просмотра на мобильных устройствах, с помощью font-size

Для того чтобы обойти трансфокации мобильными браузерами (iOS Safari, и др.) компонентов HTML формы, в тот момент, когда открывающийся список `<select>` нажат, добавьте font-size правило селектору:

```css
input[type="text"],
input[type="number"],
select,
textarea {
  font-size: 16px;
}
```

### Всплывающие подсказки

```css
.tooltip::after {
  content: attr(data-tooltip);
}
```
