FROM golang:1.20-buster

ENV TZ Asia/Tokyo
ENV LANG ja_JP.UTF-8

WORKDIR /go/src

COPY ./src /go/src

RUN go get -u github.com/cosmtrek/air && \
    go build -o /go/bin/air github.com/cosmtrek/air

CMD ["air", "-c", ".air.toml"]
