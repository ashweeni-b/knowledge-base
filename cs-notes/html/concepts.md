### Concepts in HTML

#### Basic Structure of a Web Page

```html
<!DOCTYPE html>
<html lang = "en">
    <head>
        <title> Web Page </title>
    </head>
    <body>
        <h1> Heading </h1>
        <p> Paragraph </p>
    </body>
    <footer> Footer </footer>
</html>
```

1. `<!DOCTYPE html>`
    - Represent the document type, and helps browser to display web pages correctly
    - It must only appear once at the top of the page
    - It is the first tag o the web page (before any other HTML tags)
    -It is not case-sensitive

1. `<html lang = "en">  </html>`
    
    - Root tag of an HTML page
    - Always the lang attribute must be included in the tag to declare the language of the web page

1. `<head>  </head>`

    Contains meta information about the HTML page

1. `<body>  </body>`
    
    Contains content of the web page

1. `<footer>  </footer>`

    Contains footer of the HTML page

#### HTML Elements 

- Everything from start tag to the end tag

    `<tag_name> Content </tag_name>`

- Some HTML elements have no content within it and so they are called as _empty elements_
- Empty elements do not have an end tag

#### Nested HTML Elements

HTML elements can be nested i.e. they contain other elements

> HTML is not case-sensitive

#### Attributes

- Provides additional information about HTML elements
- All HTML elements can have attributes
- Attributes are always specified in the start tag
- Attributes usually comes in name/value pairs like _name = "value"_

---