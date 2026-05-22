### Introduction to HTML

- HTML stands for _Hyper Text Markup Language_
- Defines the structure of the web page
- Component used to structure or design the web pages is known as _HTML tags_
- `index.html` is the default name for the homepage of website

#### HTML Tag

Container for some content or other HTML tags

Structure of HTML = Elements (opening and closing tags) + Content

For example:
```html
<p> This is a paragraph tag </p>
```
Here, `<p>` and `</p>` are the opening and closing tags respectively and the text within these tags is the content to be displayed on the web page

#### Basic HTML Page

```html
<!-- Tells browser that usage of HTML5 -->
<!DOCTYPE html>

<!-- Root of an HTML document -->
<html lang = "en">

    <!-- Container for metadata
     Metadata is that data that is useful but not displayed on the browser
    -->
    <head>
        <meta charset="UTF-8">

        <!-- Allows the website to be responsive on different devices -->
        <meta name="viewport" content="width=device-width, initial-scale=1.0">

        <!-- Page Title -->
        <title>Page Title </title>
    </head>

    <!-- Contains all data rendered by the browser -->
    <body>
        <!--Page Content-->
    </body>
</html>
```

#### Comments in HTML

Part of the HTML code that doesn't needs to be parsed

```html
<!---This is an example of a comment in HTML --->
```

_Note:_

1. HTML is not case-sensitive. For example, `<html>` = `<HTML>`, `<p>` = `<P>`, etc.
1. HTML tag `<html> </html>` is the parent of the head and body tags.
1. Most of the HTML elements have opening and closing tags with content in between.
1. Some tags have no content in between - `<br />`.
1. We can use inspect element or view page source to edit HTML pages.

---