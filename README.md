
# EJS Basics


| Learning Objectives |
| :---- |
| Define EJS and outline use cases |
| Implement EJS into a node.js project |
| Integration with underscore templating |
| EJS partials |



### What is EJS and what can it do for me?
**EJS** stands for Embedded Javascript.

EJS cleans the HTML out of your JavaScript with client-side templates. After EJS gets its rubber gloves on dirty code, you'll feel organized and uncluttered.

</strong><a href="http://www.embeddedjs.com/">Learn More</a>

###EJS implementation with node

<!--####Steps *(courtesy of Ilias)*

1. Install ejs: `npm install --save ejs`
2. Require it in the project: `app.set('view engine', 'ejs')`
3. Render a template: `res.render('index');`
4. Require an ejs partial *(optional)*: `<% include partials/head %>`
5. Iterate through the data *(optional)*:
 
 ```
 <% foodItems.forEach(function(food) { %>
  <li class='list-group-item'><%= food.name %>
    <span class="label label-default"><%= food.yumminess%></span>
    <button data-id="<%= food.id %>" onclick="deleteFood(this)" type="button" class="close" aria-label="Close"><span aria-hidden="true">&times;</span></button>
  </li>
<% }); %>
 ```
--> 

####Features
* Control flow: (`<% ... %>`)
* Escaped output: (`<%= ... %>`)
* Client-side support
* Static caching of intermediate JS
* Compatible with Express views

####Tags

* `<%` Scriptlet tag, for control-flow, no output
*  `<%=` Outputs the value into the template (HTML escaped)
* `<%-` Outputs the unescaped value into the template (embeddable as a string)
* `%>` Plain ending tag

#####Example
```
<% if (puppy) { %>
  <h2><%= puppy.name %></h2>
<% } %>
```

####Resources:
* [EJS on Github](https://github.com/mde/ejs)
* [EJS on NPMJS](https://www.npmjs.com/package/ejs)
* [Effective JavaScript templating](http://ejs.co/)

