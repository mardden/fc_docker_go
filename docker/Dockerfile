FROM golang:alpine

WORKDIR /usr/src/app

COPY hello.go ./

RUN go build hello.go && \
    mv hello /bin/

CMD ["hello"]
