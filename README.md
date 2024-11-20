# express-es6-template

Express template using module/ES6 syntax

After cloning the library, execute these commands to install dependencies  
`npm install`  
`npm audit fix --force`

If you do not have nodemon installed, install by executing  
`npm -g install nodemon`

**Directory and file structure**

```text
/LocalLibrary
    app.js
    /bin
        www
    package.json
    package-lock.json
    /node_modules
        [about 6700 subdirectories and files]
    /public
        /images
        /javascripts
        /stylesheets
            style.css
    /routes
        index.js
        users.js
    /views
        error.pug
        index.pug
        layout.pug
```

- **package.json** - Defines application dependencies. Defines the startup script that calls the application’s entry point, the JS file **/bin/www**

- **/bin/www** - Application’s entry point. Sets up some basic error handling and then loads app.js to do the rest of the work

- **/routes** - The app routes are stored as separate modules under this directory

- **/views** - The templates are stored under this directory

The default view installed by express is Jade. But you can choose a different template e.g. pug during your installation. The following dependencies are added by express

- [cookie-parser](https://www.npmjs.com/package/cookie-parser): Used to parse the cookie header and populate `req.cookies` (essentially provides a convenient method for accessing cookie information).
- [debug](https://www.npmjs.com/package/debug): A tiny node debugging utility modeled after node core's debugging technique.
- [morgan](https://www.npmjs.com/package/morgan): An HTTP request logger middleware for node.
- [http-errors](https://www.npmjs.com/package/http-errors): Create HTTP errors where needed (for express error handling).
