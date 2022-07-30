# apis-for-login-signup-pages-with-jwt
This is a simple login and signup page made with MEAN stack (MongoDB, ExpressJS, Angular, NodeJS).
This project includes:
User registration.
User login.
User Authorization.
Basic working of login page
When user enters email and password and when both of them are correct we return an access token (generated with jwt)
This access token is stored in localstorage of the browser.
Now if user leaves the page and opens the same site again we check to see if there is any access token present in user's localstorage.
if access token is present - > we verify that access token and redirect user to the profile page.
if access token is not present - > we keep user on the same page.
About Directories
NodeJS and ExpressJS is inside restApi/
MongoDB database is in user_db/
Angular Components are in src/app
Prerequisites to understand the project
MEAN stack (Angular 2+)
ES6 Javascript (specially promises)
JWT: Json Web Token it is a libray to generate random token it has 2 function jwt.sign() to create token and jwt.verify() to verify
bcrypt - Library to hash passwords, I've used two functions in this project bcrypt.hash() to hash password and bcrypt.compare to compare string with hashed password.
Tools / Libraries / Softwares required.
Install npm and Angular Client npm install @angular/cli (ignore if already installed)
In command prompt type npm install to download starter packages.
cd restApi and type npm install bcrypt,jsonwebtoken,mongoose,express
Install MongoDB
Go to bin folder in your mongodb directory, Mine is in c:/program files/mongodb/server/3.6/bin and type mongostore <path of user_db folder>
How to Run
Change directory to your project and ng serve to start angular server
Change directory to bin folder of your mongodb installation folder, Mine is c:/program files/mongodb/server/3.6/bin and type mongod then open new command prompt and type mongo
Change directory to restApi/ and type node index.js to start Node Server
Development server
Run ng serve for a dev server. Navigate to http://localhost:4200/. The app will automatically reload if you change any of the source files.
