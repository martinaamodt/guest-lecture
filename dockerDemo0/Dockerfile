FROM ubuntu:20.04
RUN apt-get update && apt-get install nginx -y
RUN rm /var/www/html/index.nginx-debian.html
COPY content/ /var/www/html/
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
