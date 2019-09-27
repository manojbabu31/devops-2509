# Base Image
FROM ubuntu:16.04

#Owner
MAINTAINER Manoj Babu <manojb.babu@gmail.com>

# Update the APT Repo
RUN apt-get update

# Install Apache2
RUN apt-get install apache2 -y

# Add info.html
COPY info.html /var/www/html/

# Expose server to external network
EXPOSE 80 8080

# Execute Apache2 service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"] 
