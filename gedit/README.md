# Docker

Docker file for gedit gui.

create docker file 

build docker image 

#this will make a image named firefox

> docker build -t gedit .		

#this is for loading graphical environment on docker

> xhost + local:docker                       

then run command

> docker run --rm -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix gedit
