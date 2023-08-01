#FROM fedora

#RUN mkdir /opt/tomcat/
#WORKDIR /opt/tomcat/
#RUN curl -O https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.76/bin/apache-tomcat-9.0.76.tar.gz
#RUN tar xvfz apache-tomcat-9.0.76.tar.gz
#RUN sudo dnf install --assumeyes java-1.8.0-openjdk.x86_64
#RUN java -version

#ADD petclinic.war /opt/tomcat/apache-tomcat-9.0.76/webapps

#EXPOSE 8082

#CMD ["/opt/apache-tomcat-9.0.76/bin/startup.sh,"run"]


# Use the official Tomcat image as the base image
FROM tomcat:9-jdk8

# Set the working directory to Tomcat's webapps directory
WORKDIR /opt/apache-tomcat-9.0.76/webapps

# Copy the Petclinic WAR file to the webapps directory
COPY petclinic.war ./

