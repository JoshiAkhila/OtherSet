FROM jenkins/jenkins:lts
USER root
RUN apt-get update && apt-get -y install vim
USER jenkins
COPY plugins.txt /var/jenkins_home/ 
RUN /usr/local/bin/install-plugins.sh < /var/jenkins_home/plugins.txt
