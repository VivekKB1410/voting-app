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
# testing the application
#Testing the dockerfile

#demo the feature


#testing the feature

#Hello World "Welcome"


#testing the feature

#Hello! this is testing done by VIVEK K B