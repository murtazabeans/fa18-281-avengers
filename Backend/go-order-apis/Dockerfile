FROM golang:latest 
EXPOSE 3001
RUN mkdir /app 
ADD . /app/ 
WORKDIR /app 
ENV GOPATH /app
RUN cd /app ; go get order
RUN cd /app ; go install order
CMD ["/app/bin/order"]
