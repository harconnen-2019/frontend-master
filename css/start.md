# Стартовый шаблон CSS

```css
/*------------------------------------*\
  #INIT-PROJECT
\*------------------------------------*/

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

*:where(:not(iframe, canvas, img, svg, video):not(svg *)) {
  all: unset;
  display: revert;
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
  font-size: 1rem / calc(1.4em + 0.5vw) -apple-system, BlinkMacSystemFont, Segoe
      UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans,
    Helvetica Neue, sans-serif;
}

img {
  max-width: 100%;
}

ol,
ul {
  list-style: none;
}

table {
  border-collapse: collapse;
}

textarea {
  white-space: revert;
}

a {
  text-decoration: none;
  color: inherit;
}

/*------------------------------------*\
  #SECTION-GLOBAL
\*------------------------------------*/
```
