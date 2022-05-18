FROM tomcat:8-jdk-temurin
MAINTAINER Ugander Dabbara <udabbara@cisco.com>
LABEL branchname ${branchname}
ENV TEST envtest
COPY target/maven-web-application*.war /usr/local/tomcat/webapps/maven-web-application.war
RUN echo $TEST
RUN mkdir /opt/tomcat9
ADD https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.63/bin/apache-tomcat-9.0.63.tar.gz /opt/tomcat9/
RUN yum install unzip wget git -y
CMD ["echo", "Welcome to DevOps"]
RUN "RunTwo"
ENTRYPOINT ["echo" , "ls"]
CMD ["date"]
WORKDIR /usr/local/tomcat
ARG branchName=develop
EXPOSE 80
USER udabbara
