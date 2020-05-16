# docker-jenkins
Docker file for jenkins build

Download the package and run below command to build the docker image:

cmd - # docker build -t jenkins-master:0.2 .

Run docker images to check the latest image

cmd - # docker images

Create data directory and launch the container

cmd - # mkdir /jenkins_home
cmd - # docker run -d -p 8080:8080 -p 50000:50000 -v /jenkins_home:/var/jenkins_home jenkins-master:0.2 

Check the status
cmd - # docker ps

Access jenkins:
http://localhost:8080/
