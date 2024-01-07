FROM tomsik68/xampp:latest

RUN cd /opt/lampp && \
    wget https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.zip && \
    unzip phpMyAdmin-5.1.0-all-languages.zip && \
    mv phpMyAdmin-5.1.0-all-languages phpmyadmin

EXPOSE 80 3306
CMD ["/opt/lampp/lampp", "start"]