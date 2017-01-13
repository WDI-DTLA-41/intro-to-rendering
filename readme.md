# Client side vs Server Side Rendering


# What's the difference?

Request a flat file and have the server send it back
![:static](/assets/file.png)

Request the page, then request data via ajax and render on the client.
![:client](/assets/client.png)

Requst the page, have the server render a response and send it down.
![:server](/assets/server.png)

# Templating Options

Given an array of objects

```
var list = [
    {name: 'Snoopy'},
    {name: 'Charlie Brown'}
]
```

Handlebars Syntax

```
<ul>
{{#each list}}
    <li>{{name}}</li>
{{/each}}
</ul>
```

EJS Syntax

```
<ul>
<% list.forEach(function(item) { %>
    <li><%= item.name %></li>
<% }) %>
</ul>
```

