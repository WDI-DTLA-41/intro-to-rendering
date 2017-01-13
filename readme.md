# Client side vs Server Side Rendering

![:client](/assets/client.png)
![:server](/assets/server.png)
![:static](/assets/file.png)

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

