# python-flask-helloworld
a sample hello world application using python and flask

Detailed step by step instructions

1. First, you need to install Flask. You can do that using pip by running the following command in your terminal:

pip install Flask

2. Create a new file called app.py and import the Flask library:
from flask import Flask

3. Create an instance of the Flask class:
app = Flask(__name__)

4. Define a route for the home page of your app:
@app.route('/')
def home():
    return 'Hello, World!'

5. Run the app:
if __name__ == '__main__':
    app.run(debug=True)
    
python helloworld.py

6. Navigate to http://localhost:5000 in your web browser, and you should see the message "Hello, World!" displayed on the page.


Here's the complete app.py file:

from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return 'Hello, World!'

if __name__ == '__main__':
    app.run(debug=True)

