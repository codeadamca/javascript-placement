# A Basic Introduction to Including JavaScript in an HTML Document

Much like CSS, JavaScript can be placed into an HTML document using three different mthods:

1. Inline
2. Internal
3. External

## Inline

JavaScript can be placed inside an HTML tag using an event attribute:

- onclick
- onmouseover
- onsubmit

Or inside an `href` attribute by prefixing it with `javascript:`.

Create a new HTML document, name is `inline.html`, add the standard HTML elements, and inside the `body` tag add the following code:

```html
<input type="button" onclick="alert('This is inline JavaScript!');" value="Click Me">

<br><br>

<a href="javascript:alert('This is also inline JavaScript');void(0);">Click Me</a>
```

Test the HTML file using a browser. You should see an alert message by clicking either the button or link.

## Internal

JavaScript can be placed inside an HTML document by adding JavaScript code inside a `script` tag.

Create a new HTML document, name it `internal.html`, add the standard HTML elements, and inside the `body` tag add the following code:

```html
<script>

document.write("<h1>Embedded JavaScript</h1>");
document.write("<p>This is embedded JavaScript!</p>");

</script>
```

Test the HTML file using a browser, the `body` section of the webpage should have an additional heading and paragraph.

## External

JavaScript can be placed inside an external JavaScript file. 

Create a new JavaScript file and name it external.js. When placing JavaScript inside an external JavaScript file, you do not need to include `script` tags. Add the following code:

```javascript
document.write("<h1>External JavaScript</h1>");
document.write("<p>This content comes from an external JavaScript file!</p>");
```

Next, create an HTML file, name it external.html, add the standard HTML elements, and then add the following code to the `body` section:

```html
<script src="external.js"></script>
```

Test the file using a browser, the `body` section of the webpage should have an additional heading and paragraph.

## Tutorial Requirements:

* [Visual Studio Code](https://code.visualstudio.com/) or [Brackets](http://brackets.io/) (or any code editor)

Full tutorial URL: https://codeadam.ca/learning/javascript-placement.html

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
