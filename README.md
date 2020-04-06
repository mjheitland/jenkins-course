# jenkins-course
* This is the course material for the Jenkins Course on Udemy. See https://www.udemy.com/learn-devops-ci-cd-with-jenkins-using-pipelines-and-docker/?couponCode=JENKINS_GIT


# Commands to run sonarqube project using docker-compose

Jenkins and Postgres files will be stored in $HOME/docker/*

1. cd sonarqube
2. docker-compose up
3. docker ps (should show four containers: jenkins, docker, postgres, sonarcube)
4. Get Jenkins admin password from log file: docker-compose logs -f jenkins
5. Configure Jenkins: http://localhost:8080, install suggested plugins, add "Sonarqube Scanner" plugin
6. Check Sonarqube is running: docker-compose logs -f sonarqube (might need a second run of docker-compose due to dependencies)
7. Log into SonarQube with admin/admin: http://localhost:9000, go to Account/Security and generate a token
8. In jenkins add copied token to credentials (credentials/secret text/id=sonar)
