FROM golang:alpine AS builder

WORKDIR /app

COPY ./src/ .

RUN go mod init x
RUN go build -o main .

FROM scratch
COPY --from=builder /app/main /main

CMD ["/main"]