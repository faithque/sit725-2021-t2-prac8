## The Wildfire Reporting System
---
This widlfire reporting project is the submission for Project 8 in the SIT725 course. The project is a web application  
built using ExpressJS and a MongoDB database. Project 8 introduces contaainerization using Docker for easy deployment  
setup and configuration. A Dockerfile specifying the node and file configurations necessary to create an image for our  
application and run a container for it in the Docker program was added to the project directory. A .dockerignore file  
was also included in the project.

## Installation
---
You must have Express installed to run this application in a development environment. To install Express, use the [npm install command:](https://docs.npmjs.com/getting-started/installing-npm-packages-locally)

```bash
npm install express
```

To run the tests, you must also install Moch and Chai using npm:

```bash
npm install mocha chai
```

## Usage
If you have Express installed, navigate to the project direstory (assuming you cloned it from this repository), and start the Express server  
using the following command:


```bash
npm start
```

View the website at: http://localhost:3000

To run the tests, open a new terminal and start the tests using the following command:


```bash
npm test
```

To deploy the project in Docker, open a terminal and run the following command to build an image for the project:
```bash
docker build -t <image name> .
```
To run the Docker image created, use the command:
```bash
docker run -d -p 3000:3000 <image name>
```
Once you have run that you can see the app running by using the command
```bash
docker ps -a
```
You can also stop your application by these commands
```bash
docker stop <container id>
docker rm <container id>
```
