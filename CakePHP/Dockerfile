FROM ubuntu:16.04

# Install
RUN apt-get update

RUN apt-get install -y \
	lamp-server^ \
	php-mbstring \
	php-intl \
	php-zip \
	php-dom \
	phpmyadmin \
	git

EXPOSE 8080

ENTRYPOINT ["/bin/bash"]

COPY start.sh /bin
RUN mkdir /mnt/test
RUN chmod a+x /bin/start.sh

CMD ["/bin/start.sh"]
