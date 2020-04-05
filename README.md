# jenkins-course
* This is the course material for the Jenkins Course on Udemy. See https://www.udemy.com/learn-devops-ci-cd-with-jenkins-using-pipelines-and-docker/?couponCode=JENKINS_GIT


# Commands to run sonarqube project using docker-compose
Here I am using the following folder structure:
/Users/heitlm/
  docker
  docker.sock
  jenkins_home

1. docker-compose up
2. docker ps
4. Get Jenkins admin password: docker-compose logs -f <Jenkins container id>
3. Check Sonarqube is running: docker-compose logs -f sonarqube
4. Configure Jenkins: http://localhost:8080
5. Log into SonarQube with admin/admin: http://localhost:9000
