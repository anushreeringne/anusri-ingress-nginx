#FROM alpine:3.10
#MAINTAINER Roman Safronov <electroma@gmail.com>
#COPY . /echosvc
#RUN chmod +x /echosvc/echosvc.go
#EXPOSE 8080
#ENTRYPOINT ["/echosvc"]

FROM golang:alpine
RUN mkdir /app 
ADD . /app/
WORKDIR /app 
RUN go build -o main .
RUN adduser -S -D -H -h /app appuser
USER appuser
CMD ["./main"]
