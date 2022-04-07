# DockerBasicCommands
Installing Docker on:

Mac:        https://store.docker.com/editions/community/docker-ce-desktop-mac
Windows:    https://store.docker.com/editions/community/docker-ce-desktop-windows 
Ubuntu:     sudo apt-get update
            sudo apt-get install docker.io
	   
docker --version                          checks your version of docker
docker pull <imagename>                   downloads container from dockerhub automatically 
sudo docker pull ubuntu                   downloads latest image for ubuntu on our system
sudo docker images 	                      shows images that were downloaded and the size
 
sudo docker run -it -d <imagename>
sudo docker run -it -d ubuntu
-t makes the container interactive in the terminal so that i can pass some commands
-d makes the container run as daemon in the background until i stop the container

sudo docker ps                            shows you containers current running in the system
sudo docker ps -a                         shows you a list of active and inactive containers 

sudo docker stop <containerID>            stops the container
sudo docker stop r456fgh466

Sudo docker kill <containerID>            in case stop command doesn’t work 
Sudo docker kill r456fgh466

sudo docker run -it -d ubuntu             starts the container

sudo docker rm <containerID>              deletes the container from the system
sudo docker rm r456fgh466

sudo docker rmi <imageID>                 removes the image from the system
sudo docker rmi <4567890>

sudo docker exec <containerID>            allows you to work with the container
sudo docker exec r456fgh466

sudo docker exec-it <containerID> bash    allows you to get inside the container
sudo docker exec-it r456fgh466 bash          
-t makes the container interactive in the terminal so that i can pass some commands
bash I want to run container in current terminal space i’m working on which is bash

apt-get update starts updating the container as it’s a new operating system running on the system

sudo docker ps  (need to run docker because it’s a new machine now)
sudo docker ps  (need to install sudo library as it’s not installed in container) 
