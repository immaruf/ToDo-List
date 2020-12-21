# Simple ToDo List App Using `MongoDB`, `express`, `Nodejs`, `EJS`
* NodeJS- For rendering the Server side handling of GET and POST requests and connecting to DB
* MongoDB- The User data are saved in a Mongo Database deployed on AWS via MongoDB
* ExpressJS- For passing the data from user to DB and vice versa.
* EJS- For rendering the data from user to DB and vice versa on the webpages.
* NPM Packages- Various other NPM packages like Body-Parser etc
* It supports `CRUD` operation to a todo task
* Communication between browser and server is established.

[Live Demo- Click Here!](https://my-t0d0-l1st.herokuapp.com/)

## RUN
### Running locally
```
$ git clone https://github.com/immaruf/ToDo-List.git
$ cd ToDO-List
$ npm i
$ mongod  
    # if you don't have mongodb installed, use $ apt-get install mongodb
$ node app.js
```
now you can use this app via [http://localhost:3000/](http://localhost:3000/)
<br>
### DEPLOY to HEROKU
#### Prerequisites for Heroku
* An Heroku account
```
$ heroku login
$ heroku create
    # For the first time you deploy: create heroku app, heroku create git remote for you named 'heroku'

$ git push heroku HEAD:master
    # push current commit to remote then deploy automatically
    # NOTE heroku in default deploy only when you push to heroku/master

$ heroku ps:scale web=1  # specify hardware resource
$ heroku open            # browse website
```
* other management commands
```
$ heroku logs            # view logs
$ heroku config | grep MONGODB_URI   # check heroku mongo uri
$ heroku rename NEW_APP_NAME         # rename app (optional)
$ git remote set-url heroku https://YOUR_NEW_HEROKU_GIT_REPO_URL.git
    # don't forget to update remote after renaming
```
now you can use this app via `http://MY_HEROKU_APP_NAME.herokuapp.com/`
