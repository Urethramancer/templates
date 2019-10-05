FROM golang:alpine AS builder
RUN apk update && apk add --no-cache git
ADD . /src
RUN cd /src && go get -d -v && CGO_ENABLED=0 GOOS=linux go build -a -ldflags "-w -s" -o server .

FROM scratch
WORKDIR /app
COPY --from=builder /src/server /app/server
ENTRYPOINT ["/app/server"]
