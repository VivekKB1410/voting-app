FROM golang:alpine as builder
LABEL maintainer="mgdevstack" \
    vendor="Zettabytes" \
    owner="zbio"
ADD main.go  .
RUN GO111MODULE=off CGO_ENABLED=0 GOOS=linux go build -o app

FROM alpine
LABEL maintainer="mgdevstack" \
    vendor="Zettabytes" \
    owner="zbio"
COPY --from=builder /go/app /app
ENTRYPOINT ["/app"]
#Testing roost git operations
# test

#Testing git ops feature


#Testing Jenkins build