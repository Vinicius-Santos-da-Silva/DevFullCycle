FROM golang:1.12-alpine AS build_base

# Set the Current Working Directory inside the container
WORKDIR /tmp/go-sample-app

COPY ./hello_server.go .



# Build the Go app
RUN go build -o ./out/go-sample-app .


# Start fresh from a smaller image
# FROM alpine:3.9 
FROM scratch

COPY --from=build_base /tmp/go-sample-app/out/go-sample-app /app/go-sample-app

# RUN rm -rf /tmp/go-sample-app

CMD ["/app/go-sample-app"]


# docker build . -f Dockerfile -t vsantos98/golang-2mb
# docker run vsantos98/golang-2mb


# docker build . -f Dockerfile -t vsantos98/codeeducation
# docker run vsantos98/codeeducation