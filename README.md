# ToDo-List
[Link- Click Here!](https://my-t0d0-l1st.herokuapp.com/)

## Its a TodoList webapp where people can make a list of tasks and edit it accordingly.
### Tech-Stack
* NodeJS- For rendering the Server side handling of GET and POST requests and connecting to DB
* MongoDB- The User data are saved in a Mongo Database deployed on AWS via MongoDB
* ExpressJS- For passing the data from user to DB and vice versa.
* EJS- For rendering the data from user to DB and vice versa on the webpages.
* NPM Packages- Various other NPM packages like Body-Parser etc
### Running locally
```
$ git clone https://github.com/immaruf/ToDo-List.git
$ cd todo_list_mean
$ npm i
$ mongod  
    # if you don't have mongodb installed, use $ apt-get install mongodb
$ node app.js
```
