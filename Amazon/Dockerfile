# Use official Tomcat base image
FROM tomcat:9.0-jdk17

# Clean default webapps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy the WAR file from your repo structure into Tomcat webapps
COPY Amazon/Amazon-Web/target/Amazon.war /usr/local/tomcat/webapps/ROOT.war

# Expose port
EXPOSE 8080

# Run Tomcat server
CMD ["catalina.sh", "run"]
