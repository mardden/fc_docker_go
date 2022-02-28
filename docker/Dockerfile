FROM golang:alpine AS builder

WORKDIR /usr/src/app

COPY hello.go ./

RUN go build hello.go


FROM scratch

WORKDIR /

COPY --from=builder /usr/src/app/hello /bin/

CMD ["hello"]
