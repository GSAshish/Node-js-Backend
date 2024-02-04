
```bash
npm install --save ejs
```



```js
// set a global config value like you can set keys also like env keys
//  like setting the current user we can use this
app.set("view engine","pug");
// to tell what is view file
app.set("views","<name of your view file>");
app.set('view options', { delimiter: '{{' });

// pug is a supported automatically 
```

```html
<h1><%= title %></h1>
<% if (condition) { %>
<% for (var i = 0; i < items.length; i++) { %>
<div><%- rawHtml %></div>
```


partials

```html
<%- include('partialName') %>
```


header.ejs
```html
<!-- header.ejs -->
<header>
  <h1>My Website</h1>
</header>

```

```html
<!-- index.ejs -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title><%= title %></title>
</head>
<body>
  <%- include('header') %>
  <h1><%= title %></h1>
  <p>Welcome to my website!</p>
</body>
</html>

```