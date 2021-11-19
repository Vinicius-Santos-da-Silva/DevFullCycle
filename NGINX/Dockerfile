FROM nginx:latest

COPY html /usr/share/nginx/html

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "nginx", "-g" , "daemon off;" ]


# docker build -t vsantos98/nginx:prod . -f Dockerfile.prod

# docker run -d --network laranet --name nginx -p 8080:80 vsantos98/nginx:prod