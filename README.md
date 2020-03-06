package.json

    npm configuration file.

server.js

    Activates the routes and opens the port for the website.
config.json

    json file containing configuration information for MySQL database access.

passport.js

    unknown

middleware/isAuthenticated.js

    Helper for html-routes.js. Returns information that allows html-routes.js to know whether the user is logged in or not.

index.js

    gathers up .js files in the /models directory and creates connections to all defined databases.

user.js

    provides definitions for mysql database.

login.html

    user logs in with email and password combination. Uses login.js for functionality.

members.html

    User sees this page after logging in or creating account. Currently a placeholder displaying a greeting to the user. Uses members.js for functionality.

signup.html

    User signs up with email and password combination. Uses signup.js for functionality

js/login.js

    helper for login.html page. It calls the login API and redirects to members.html if successful.

js/members.js

    helper for members.html page. In current version of page it retrieves the user's email address.

js/signup.js

    helper for signup.html page. It calls the login API and redirects to members.html if successful.

stylesheets/style.css

    Stylesheet for the HTML pages.
api-routes.js

    routes API calls to the database.

html-routes.js

    routes website calls. If a user access /members without logging in they will be redirected to the signup page.