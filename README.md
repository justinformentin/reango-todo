# React + Redux and Django To Do

This project shows Django, Django Rest Framework, React, and Redux working together. It also utilizes hot reloading via webpack.

It's based on [Dan Abromov's todomvc example](https://github.com/gaearon/redux-devtools), which you can find [**here.**](https://github.com/reduxjs/redux-devtools/tree/master/examples/todomvc)

## Usage

Clone the project and cd into it.
```
git clone https://github.com/justinformentin/reango-todo.git && cd reango-todo
```
Then, create a virtualenv, activate it, and install the requirements.
```
virtualenv env && source env/bin/activate && pip install -r requirements.txt
```
Next, cd into the project.
```
cd todomvc
```
Install the dependencies.
```
npm install
```
Create the database and create the superuser.
```
./manage.py migrate && ./manage.py createsuperuser
```
Now, open another terminal in the same directory location.

In one terminal, start the server.
```
./manage.py runserver
```
In the second terminal, start the client.
```
npm start
```
You should now be able to login via localhost:8000/admin

View the app at the root: localhost:8000, and the api at localhost:8000/api

#### Note

1. If you're on windows, instead of ./manage.py migrate you need to use 
```
python manage.py migrate
```

2. The React components are in the client directory, and django is in the server directory.

