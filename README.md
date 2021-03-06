# simple-flask-react-template
# An application template in Python, Flask and ReactJS.

## Main Technologies:
* Python
* pip
* Flask
* Javascript
* ReactJS
* NPM
* webpack
* CSS
* Docker

## Building the application:

Option 1: python server  
1) use pip to install the requirements of the server:  
$ pip install -r requirements.txt  
Obs.: I highly recommend to use a virtual env to avoid dependency conflicts.

2) change directory to static folder:  
$ cd static

3) install front end dependencies:  
$ npm install  
(dev-only):  
$ npm i webpack --save-dev  
$ npm i babel-core babel-loader babel-preset-es2015 babel-preset-react --save-dev  
$ npm i react react-dom --save-dev

4) build the front end:  
$ npm run build  
Obs.: You can use 'npm run watch' to avoid building the front end everytime a change is made.

5) change to main directory:  
$ cd ..

6) run the server:  
$ python server.py

7) access via browser http://localhost:5000 and you are good to go :)


Option 2: Docker  
1) build the application:  
$ docker-compose build

2) run the server:  
$ docker-compose up

3) access via browser http://localhost:5000 and you are good to go :)

