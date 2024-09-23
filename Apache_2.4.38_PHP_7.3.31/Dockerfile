FROM debian:buster

RUN apt update && apt -y upgrade

RUN apt-get install systemd -y

RUN apt-get install wget curl unzip net-tools vim -y

RUN apt -y install php php-common
RUN apt -y install php-cli php-fpm php-json php-pdo php-mysql php-zip php-gd  php-mbstring php-curl php-xml php-pear php-bcmath
RUN apt -y install libapache2-mod-php
RUN a2enmod php7.* 

COPY ./info.php /var/www/html/

WORKDIR /var/www/html

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]
