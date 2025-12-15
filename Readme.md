# Python Application using Dockerfile
 ## Project Overview

This project demonstrates how to containerize a simple Python application using a Dockerfile. Docker allows you to package your application along with its dependencies so it runs consistently across different environments

### Basic Requirements:
python-docker-app/

│── app.py
│── requirements.txt
│── Dockerfile


## Step-By-Step

### Step 1:- Launch Instance
- Add port 5000 in the security group

![](./Img/1.png)
### Step 2:- Connect to server
![](./Img/2.png)
### Step 3:- Update package
- sudo apt update
![](./Img/3.png)
### Step 4:- Install docker
- sudo apt install docker.io -y

![](./Img/4.png)
### Step 5:- Create one directory and 3 files
- sudo su
- mkdir python-app
- app.py, dockerfile, requirements.txt

![](./Img/5.png)
#### 1. Dockerfile

![](./Img/6.png)
#### 2. app.py

![](./Img/7.png)
#### 3. requirements.txt

![](./Img/8.png)
### Step 6:- Build docker image
-  docker build -t myappimg .

![](./Img/9.png)
### Step 7:- Run the container
- docker run -d -p 80:5000 --name myapp myappimg

![](./Img/10.png)
### step 8:- Access using ip
![](./Img/11.png)

## Conclusion

This project helps understand the basics of Docker by containerizing a simple Python application. It is a great starting point for learning Docker and container-based deployments.
