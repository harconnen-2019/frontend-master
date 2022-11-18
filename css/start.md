# Стартовый шаблон CSS

```css
:root {
  --primary: #0275d8;
  --success: #5cb85c;
  --info: #5bc0de;
  --warning: #f0ad4e;
  --danger: #d9534f;
  --light: #f7f7f7;
  --dark: #292b2c;

  --sm: 640px;
  --md: 768px;
  --lg: 1024px;
  --xl: 1280px;
  --2xl: 1536px;
}

html {
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  font-size: 1rem/1.4em -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
    Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
}

img {
  max-width: 100%;
}

a {
  text-decoration: none;
  color: inherit;
}
```
