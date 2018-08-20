
# Node Server (Express + Sqlite + Sequelize + Nodemon)



<h3>Start in debugging mode</h3>

  Mac OS/Linux 

  ``` $ DEBUG=myapp:* npm start ```

  Windows 

  ``` set DEBUG=myapp:* & npm start``` 


<h3>Start without debugging mode</h3>

  ``` npm start``` 


Open up following URL http://localhost:3000 in your browser


<h3> Create sqlite databases </h3>

Just enter ```node create_db```, it will create Databases ( development, testing, production )

<h3> Create all tables, defined in ./models folder </h3>

By entering ```node create_tables``` it will look for sequelize-models defined in models folder, and create them. 
( The force : true attribute does override existing tables ) 

<h3> Route /users </h3>

| Route        | HTTP-Method | Body-Object (key-values) | Result  |
| ------------- |:-------------:| -----| ------------- |
| /users      | GET | - |Gets all users available |
| /users/2      | GET | -  |  Gets user with Id 2   |
| /users |      POST      |  { "firstname" : String  "lastname" : String "username" : String }  | Create a new user
| /users/2 |      DELETE      |  -  | Delete user with id 2
| /users/3 |      PUT      |  { "firstname" : String  "lastname" : String "username" : String }  | Update user with id 3



