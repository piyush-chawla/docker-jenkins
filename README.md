# docker-jenkins
Docker file for jenkins build

Download the package and run below command to build the docker image:

# docker build -t jenkins-master:0.2 .

Run docker images to check the latest image

# docker images

Create data directory and launch the container

# mkdir /jenkins_home
# docker run -d -p 8080:8080 -p 50000:50000 -v /jenkins_home:/var/jenkins_home jenkins-master:0.2 

Check the status
# docker ps

Access jenkins:
http://localhost:8080/
