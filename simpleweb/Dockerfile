# Use a base image that supports Tomcat 10 and Java 21
FROM tomcat:10.1-jdk21

# Remove default webapps to keep the container clean
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy the WAR file to the webapps directory
COPY target/simpleweb.war /usr/local/tomcat/webapps/

# Expose the port that Tomcat is running on
EXPOSE 8080
