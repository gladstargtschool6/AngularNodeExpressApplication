https://github.com/praorane/AngularNodeExpressApplication.git  This repo aims primary walkthrough to bind Nodejs and AngularJs for a SPA. Connection to Mongo or any other server data is substituted by static data from api facade.  To get the Node project structure in place, one can refer to http://expressjs.com/starter/generator.html  The source code is structured as : . ├── app.js ├── bin │   └── www ├── package.json ├── public │   ├── images │   ├── javascripts │   └── stylesheets │       └── style.css ├── routes │   ├── index.js │   └── users.js └── views     ├── error.jade     ├── index.jade     └── layout.jade  Angular code is accomodated in this structure. Templates or views are part of views/partials folder. Front end business and routing code is moved to public/js folder path.  The navigation is from app.js -> which includes Node set up logic. Also the API call paths are regitered in app.js. Actual database manipulation is included in api.js.  When the application launches, app.js initializes the node serve and redirects to views/index.jade. From index.jade we use the angular routing of public/js/app.js and renders partial views found in views/partials folder.
