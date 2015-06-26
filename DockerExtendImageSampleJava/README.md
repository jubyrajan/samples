# Docker extension image sample

A simple example on creating a docker image by extending another. The extended image extends the standard docker image *java*, add a simple HelloWorld.java program which can be compiled and executed from the new extended image.

Prerequisite: Install Docker

Get java docker image: **sudo docker pull java**

Get the Docker image for java extension image: ** wget https://raw.github.com/jubyrajan/samples/master/DockerJavaHelloWorld/Dockerfile **

Build Docker Image: **sudo docker build -t "java_ext_test" .**

Check the newly created image: **sudo docker images**

Run Docker Image Interactively: **sudo docker run -it --rm java_ext_test**

Compile and execute inside Docker Container

- javac HelloWorld.java
- java HelloWorld


Remove the java_ext_test docker image if required: **sudo docker rmi java_ext_test**
