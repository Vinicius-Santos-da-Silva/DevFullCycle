FROM mohsenmottaghi/php-fpm-zts

WORKDIR /app

RUN apt-get update
RUN apt-get install vim -y
RUN apt install nginx -y
RUN nginx

COPY html/ /var/www/html


EXPOSE 80

# ENTRYPOINT [ "nginx" ]
# ENTRYPOINT [ "echo" , "Hello" ]
# CMD [ "Hello" ]
# Este parametro vai para o entrypoint