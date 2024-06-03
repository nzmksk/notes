## CSS in HTML
- CSS can be added to HTML documents in 3 ways:
  - **Inline** - using `style` attribute inside HTML elements.
  - **Internal** - using `<style>` element in the `<head>` section.
  - **External** - using `<link>` element to link to an external CSS file.

### Inline CSS
- Used to apply style to a single HTML element.

Example:
```html
<h1 style="color:blue;">A Blue Heading</h1>
```

### Internal CSS
- Used to define a style for a single HTML page.

Example:
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {background-color: powderblue;}
      h1   {color: blue;}
      p    {color: red;}
    </style>
  </head>
  <body>
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
  </body>
</html>
```

### External CSS
- Used to define a style for many HTML pages.

Example:
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
  </body>
</html>
```
`styles.css`:
```css
body {
  background-color: powderblue;
}

h1 {
  color: blue;
}

p {
  color: red;
}
```

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
| [Quotations](./05-quotations.md) | [HTML Introduction](./01-introduction.md) |  |