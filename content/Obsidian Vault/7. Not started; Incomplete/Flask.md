2024-07-3120:10
Status: #Incomplete  
### FLASK

Web frameworks make the process of typing code manually much easier. Popular frameworks include Django, Pyramid, Jinja and Flask. (Basically a library). HTML’s major fault is that it is static. By incorporating Python, you can make web pages more dynamic.

```python
#Displaying time example
from flask import Flask 
from datetime import datetime 
from pytz import timezone
#importing function Flask and module
app = Flask(_name_) 
#from here define application behaviours 
@app.route("/") 
def time():
	now = datetime.now(timezone('America/New_York'))
	return "The current date and time in Cambridge is {}".format(now) 
```

The way that Python is implemented into HTML is through the usage of decorators. A decorator is a function that takes in another function as a parameter and then returns a function. In Flask they are used to associate a particular function with a particular URL.

```python
#Running a Flask application within CS50 IDE 
export FLASK_APP=application.py 
	export FLASK_DEBUG=1
		flask run 
```

```python
#Passinng data via URLs is akin to using HTTP GET 
@app.route("/show/<number>")
def show(number):
	return "You passed in {}".format(number) 
```

```python
#Passing data via HTML forms as with HTTP POST (must indecate the acception of POST) 
@app.route("/login",methods=['GET','POST'])
def login()
	if not request.form.get("username") 
		return apology("must provide username")
```

```python
url_for()
redirect()
session()
render_template()
```

→ Flask Guide: [](https://flask.pocoo.org/docs/0.12/quickstart/)[https://flask.pocoo.org/docs/0.12/quickstart](https://flask.pocoo.org/docs/0.12/quickstart)

→ Jinja Guide: [https://jinja.pocoo.org](https://jinja.pocoo.org)

### AJAX

AJAX (formerly known as Asynchronous JavaScript and XML(JSON)) Allows us to dynamically update a webpage. For example the scores of a sports game are updated using AJAX

XMLHttpRequests allow a client to ask for an asynchronous request for more information. Syntax is as follows: var xhttp = new XMLHttpRequest();. After obtaining the new object, you need to define its onreadystatechange behavior. This is a function (typically an anon function) that will be called when the asynchronous HTTP request has completed, and thus typically defines what is expected to change on your site. They have two additional properties that are used to detect when the page is finished loading.

- The readyState property will change from state=0 (request not yet initialized) to 1,2,3 and 4(request finished, response ready); Returning 200 (OK)

Then ensure asynchronous request using open() method to define the request and the send() method to actually send it. → There is a slightly different way to do this in jQuery

```python
function ajax_request(argument)
{
	var aj = new XMLHttpRequest();
	aj.onreadystatechange = function() {
		if (aj.readyState == 4 && aj.status == 200) 
	#do something to the page here
	};
	aj.open("GET",/*url*/,true);
	aj.send();
}
```

This can be done in jQuery: [https://api.jquery.com/jquery.ajax/](https://api.jquery.com/jquery.ajax/)

vsco

css files

[](https://www.example.com/route)[https://www.example.com/](https://www.example.com/)route/?key=value

flask framework in python

[app.py](http://app.py)

requirements.txt

static/

templates/

decorator

Advantages to using flask

URLs

templates

input tag

form tag

key value pair

jinja

privacy + inspect

post

confirm form resubmission

MVC

select menu

cross site request forgery

OS.environ

band

sending emails through python

cookies

sessions

shopping carts

post

fetch

JSON

# Source(s)