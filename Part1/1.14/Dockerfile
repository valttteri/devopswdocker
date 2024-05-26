# backend
FROM golang:1.16 

WORKDIR /usr/src/app 

COPY . . 

ENV REQUEST_ORIGIN=http://127.0.0.1:5000

RUN go build 

EXPOSE 8080 

CMD ["./server"] 

# frontend
FROM ubuntu:latest

WORKDIR /usr/src/app

RUN apt-get update && apt-get -y install curl

RUN curl -sL https://deb.nodesource.com/setup_16.x | bash

RUN apt-get install -y nodejs

COPY . . 

EXPOSE 5000 

ENV REACT_APP_BACKEND_URL=http://127.0.0.1:8080

RUN npm install 

RUN npm run build 

RUN npm install -g serve 

CMD ["serve", "-s", "-l", "5000", "build"]