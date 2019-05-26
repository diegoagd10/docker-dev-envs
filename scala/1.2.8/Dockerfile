FROM centos

# Updating system
RUN yum update -y 

# Installing dependencies
RUN yum install -y sudo zip unzip curl

# Installing java
RUN sudo yum install -y java-1.8.0-openjdk-devel

# Installing sbt
RUN curl https://bintray.com/sbt/rpm/rpm | sudo tee /etc/yum.repos.d/bintray-sbt-rpm.repo
RUN sudo yum install -y sbt-1.2.8