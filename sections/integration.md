[<<<Back](css_basic.md) | [Next>>>](rules.md)

# Integrating CSS and HTML

In order for CSS to inform the style of the content on the page, it must be integrated with your HTML. CSS can be integrated into your HTML in three ways: inline, internal, and external.

## Option one: inline

Inline styling adds CSS directly into the HTML of a page to adjust the style of particular parts of a page. 

For example, if you want the text of your first paragraph to be red, but the text of your second paragraph to be blue:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>About</title>
  </head>
  <body>
    <p style="color: red">
      Content of paragraph
    </p>
    <p style="color: blue">
      Content of paragraph
    </p>
  </body>
</html>
```

## Option two: internal

Internal styling also adds CSS directly into the HTML, but keeps it separate from the content code of the page by adding it into the head using the `<style>` tag. When using internal styling you are providing styling rules for the entire page. For example, if you want all headings to be blue:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>About</title>
    <style>
     h1 {
       color: blue;
     }
    </style>
  </head>
  <body>
    <h1>
      Heading One
    </h1>
    <p>
      Content of paragraph
    </p>
    <h1>
      Heading Two
    </h1>
    <p>
      Content of paragraph
    </p>
  </body>
</html>
```

## Option three: external

External styling creates a completely separate document for your CSS that will be linked to your HTML in the head section of your HTML document using the code below. This separate document is called a **stylesheet** and should be named `style.css`. This document must be stored in the same folder as the HTML document it is linked to.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>CSS Example</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
  </body>
</html>
```

## Best practices

Option 3, external styling, is preferred by most web developers because it's more manageable and because it lends itself to greater consistency across the entire site.

To link your stylesheet with your `index.html` file, insert the following code into the head element:

```html
<link rel="stylesheet" href="style.css">
```

[<<<Back](css_basic.md) | [Next>>>](rules.md)
