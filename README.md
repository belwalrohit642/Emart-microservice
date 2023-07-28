# Microservice Project

Deployment of a microservice application(Emart). This application was designed by using microservice architecture.

In the frontend, you have an API gateway created with Nginx and this listens at three end points, /root,/api,/webapi. When the user access the URL of the website,it will be redirected to root,which is an app written in Angular, this will give the frontend and also called client app. And this will in turn connect to /api,which will se served by an application Emart api written in node.js and it also needs mongodb database.This application also has a webapi,which connects to an application books API which is written in java and this also needs a MYSQL database.
																																																								
So all these app such as  Nginx,Angular,node.js,java,mongo,MYSQL all these will be containers.


Login to the VM using Vagrantfile<br>
vagrant up<br>
vagrant ssh<br>

#Clone source code of Emart App<br>
git clone https://github.com/devopshydclub/emartapp.git<br>
ls<br>
cd emartapp/<br>
ls<br>

#Bring up  containers from docker-compose file<br>
vim docker-compose.yaml<br>
docker-compose up -d<br>
docker ps<br>
ip addr show<br>
<br>
#Go to browser enter http://VMIp:80<br>

#Clean up<br>
docker-compose down<br>



