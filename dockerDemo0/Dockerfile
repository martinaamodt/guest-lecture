# Image base
FROM ubuntu:20.04
# Install nginx
RUN apt-get update && apt-get install nginx -y
# Remove old index
RUN rm /var/www/html/index.nginx-debian.html
# Add my own content
COPY content/ /var/www/html/
# Start nginx in the foreground
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
