# <%= EJS %>
## Embedded JavaScript templating

### What is EJS?

is a simple templating language that lets you generate HTML markup with plain JavaScript.

![image](https://images.g2crowd.com/uploads/product/image/social_landscape/social_landscape_f9dd821cb48125c63c64b6f5c7552372/ejs.png)


### Features :

* Fast compilation and rendering
* Simple template tags: <% %>
* Both server JS and browser support
* Complies with the Express view system

### Tags 

* <% 'Scriptlet' tag, for control-flow, no output
* <%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
* <%= Outputs the value into the template (HTML escaped)
* <%- Outputs the unescaped value into the template
* <%# Comment tag, no execution, no output
* <%% Outputs a literal '<%'
* %> Plain ending tag

### Is EJS a framework?
Now, the first thing we need to do is to set EJS as our templating engine with Express which is a Node. js web application server framework, which is specifically designed for building single-page, multi-page, and hybrid web applications. It has become the standard server framework for node. js

### How to run EJS :

1. Install. It's easy to install EJS with NPM. $ npm install ejs.
2. Use. Pass EJS a template string and some data. BOOM, you've got some HTML. ...
3. Browser support. Download a browser build from the latest release, and use it in a script tag.


