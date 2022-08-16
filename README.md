## Flask framework + Jinja 
### What is Flask?

Flask is a micro web framework written in Python. 
It is classified as a microframework because it does not require particular tools or libraries.

It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions. 

However, Flask supports extensions that can add application features as if they were implemented in Flask itself. 

Extensions exist for object-relational mappers, form validation, upload handling, various open authentication technologies and several common framework related tools.

Flask has become popular among Python enthusiasts. 

As of October 2020, it has second most stars on GitHub among Python web-development frameworks, only slightly behind Django.

### Flask components

* Werkzeug (German for "tool")

Is a utility library for Python for Web Server Gateway Interface (WSGI) applications.
It can instantiate objects for request, response, and utility functions.

* Jinja

Is a template engine for the Python programming language. 
Similar to the Django web framework, it handles templates in a sandbox.

* MarkupSafe

Is a string handling library for the Python programming language. 
The eponymous MarkupSafe type extends the Python string type and marks its contents as "safe";
combining MarkupSafe with regular strings automatically escapes the unmarked strings, while avoiding double escaping of already marked strings.
* 
* ItsDangerous

Is a safe data serialization library for Python. It is used to store the session of a Flask application in a cookie without allowing users to tamper with the session contents. 

### What is Jinja

Jinja is a fast, expressive, extensible templating engine. 
Special placeholders in the template allow writing code similar to Python syntax. 
Then the template is passed data to render the final document

### Using flask


#### set virtual env
Virtual env keeps all required libraries loaded and a set of pre-requisites for you app. 

This keeps dependencies isolated from other apps. 

There are a few virtual env managers, the most common are:
* conda
* pip
* pyenv


In order to create virtual env,  you need  to execute this command on a terminal.
```shell
py -m venv env
```

activate virtual env (Windows)
```shell
./env/Scripts/activate.bat
```

activate virtual env (Mac)
```shell
source env/bin/activatee
```

deactivate virtual env
```commandline
deactivate
```

### Setting up a Flask app
installing Flask
```shell
pip install flask
```

configure flask
```shell
export FLASK_ENV=development
export FLASK_APP=hello
```

#### Running flask app

Execute next commands in Terminal/console
```shell
export FLASK_ENV=development
export FLASK_APP=app_name
flask run
```

If everything goes as expected you will get an output like this
```shell
Output
 * Serving Flask app "app_name" (lazy loading)
 * Environment: development
 * Debug mode: on
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: XXX-XXX-XXX
```

## Useful links

* https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
* https://flask.palletsprojects.com/en/2.2.x/
* https://jinja.palletsprojects.com/en/3.1.x/
* https://www.digitalocean.com/community/tutorials/how-to-make-a-web-application-using-flask-in-python-3-es


## Next steps:

### Security
* https://www.loginradius.com/blog/engineering/guest-post/securing-flask-api-with-jwt/

### ORM
* https://www.section.io/engineering-education/flask-database-integration-with-sqlalchemy/
* https://flask.palletsprojects.com/en/1.1.x/patterns/sqlalchemy/

### Error Handling (HTTP)
* https://flask.palletsprojects.com/en/2.2.x/errorhandling/#error-handlers

### Unit tests
* https://codethechange.stanford.edu/guides/guide_flask_unit_testing.html
* https://testdriven.io/blog/flask-pytest/