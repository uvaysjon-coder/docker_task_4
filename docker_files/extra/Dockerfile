FROM ubuntu:20.04
ARG DEBIAN_FRONTEND=noninteractive
ENV DEVOPS="Changed"
RUN apt-get -y update
RUN apt-get -y install apache2

RUN echo "Environment variable:" $DEVOPS > /var/www/html/index.html

CMD ["/usr/sbin/apache2ctl", "-D" "FOREGROUND"]
EXPOSE 80