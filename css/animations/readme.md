# Анимация CSS

---

## Добавляем анимацию пишущей машинки CSS

```html
<body>
  <header>
    <h1>This is a Header</h1>
  </header>
</body>
```

Теперь стилизуем. Добавляем мигающий курсор в конце текста с помощью свойства border-right:

```css
header h1 {
  font-size: 70px;
  font-weight: 500;
  color: #553c9a;
  border-right: 4px solid #000; /*This will be the blinking cursor*/
}
```
