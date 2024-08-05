FROM golang:1.20

WORKDIR /app

COPY . .

ENV REQUEST_ORIGIN http://localhost:5001

RUN go build

CMD ./server

#CMD [ "serve", "-s", "-l", "5001", "build" ]