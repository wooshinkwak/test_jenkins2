# Base image
FROM tomcat:9.0

# Maintainer
LABEL maintainer="star901210@hanmail.net"

# Remove default webapps
RUN rm -rf /usr/local/tomcat/webapps/*

# Add WAR file to Tomcat webapps directory
COPY target/ROOT.war /usr/local/tomcat/webapps/ROOT.war

# Expose port 8080
EXPOSE 8080

# Start Tomcat
CMD ["catalina.sh", "run"]
