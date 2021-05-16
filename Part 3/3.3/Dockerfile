FROM golang:alpine

ENV REQUEST_ORIGIN=localhost:5000

RUN go build \
    useradd -m frontenduser \
    ./server
    
WORKDIR $APP_HOME

EXPOSE 8080

USER frontenduser
