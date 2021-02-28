# EJS Partials 

- They are particularly useful for reusing the same markup between different views, layouts, and even other partials.


- Partials are rendered synchronously, so they will block Sails from serving more requests until they're done loading.  
 It's something to keep in mind while developing your app, especially if you anticipate a large number of connections.


- Built-in support for partials in Sails is only for the default view engine, ejs.  
