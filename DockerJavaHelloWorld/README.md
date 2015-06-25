# samples
Install Docker

Get java docker image: *sudo docker pull java*

Get the Docker image for java extension image: *wget https://raw.github.com/jubyrajan/samples/master/DockerJavaHelloWorld/Dockerfile*

Build Docker Image: *sudo docker build -t "java_ext_test" .*

Check the newly created image: *sudo docker images*

Run Docker Image Interactively: *sudo docker run -it --rm java_ext_test*

Compile and execute inside Docker Container

- [x] javac HelloWorld.java
- [x] java HelloWorld


Remove the java_ext_test docker image if required: *sudo docker rmi java_ext_test"*
