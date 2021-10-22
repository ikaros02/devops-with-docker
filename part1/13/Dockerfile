FROM golang:1.16-alpine

WORKDIR /src/usr/app/
COPY ./example-backend .

RUN go build

CMD ["./server"]

EXPOSE 8080