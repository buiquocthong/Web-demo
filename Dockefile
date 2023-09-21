# Use a lightweight base image
FROM tomcat:11.0-jdk21-openjdk-slim

# Remove the default Tomcat apps
RUN rm -rf /usr/local/tomcat/webapps/ROOT
RUN rm -rf /usr/local/tomcat/webapps/examples

# Add your HelloWorld.war to the webapps directory
ADD ROOT.war /usr/local/tomcat/webapps/

# Expose port 8080
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]