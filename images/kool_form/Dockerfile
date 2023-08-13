FROM ubuntu:latest
LABEL "Author"="Keiran"
LABEL "Project"="Kool"
RUN apt update
RUN apt install apache2 -y
RUN apt install git -y
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD kool_form.tar.gz /var/www/html

