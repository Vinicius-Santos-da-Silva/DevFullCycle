# docker build -t vsantos98/nodejs-with-nginx:prod . -f Dockerfile.prod

# docker run -d --network laranet --name nodejs vsantos98/nodejs-with-nginx:prod
# Ou
# docker run -d --network laranet --name nodejs-with-nginx -p 3000:3000 vsantos98/nodejs:prod