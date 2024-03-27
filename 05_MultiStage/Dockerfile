#---- stage 1 ----
FROM golang:alpine AS builder

WORKDIR /go/src/app
COPY main.go .

RUN go mod init 
RUN go build -o webserver .

CMD ["./webserver"]

#---- stage 2------
FROM scratch

WORKDIR /app
COPY --from=builder /go/src/app /app/

# EXmaple
RUN apt update && apt install -y nginx pkg2
RUN apt install -y nginx
RUN apt install -y pkg2


CMD ["./webserver"]