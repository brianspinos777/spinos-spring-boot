# Views


###### /src/main/resources/static/foo.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <script src="scripts/foo.js"></script>
    <link rel="stylesheet" href="styles/foo.css">
</head>
<body>
    <h1>Hello from foo</h1>
</body>
</html>
```


###### /src/main/resources/static/scripts/foo.js
```js
alert("foo");
```


###### /src/main/resources/static/styles/foo.css
```css
body {
    color: red;
}
```


###### Browser
```
http://localhost:8080/foo.html
```

