# ==== Using the image alpine 3.22 for smaller image size ====== # 
FROM golang:alpine3.22

# setting the workdirectory as root 
WORKDIR /app

# Copying the go code to the image #
COPY ./dispatcher.go /app/

RUN go build dispatcher.go

CMD ["./dispatcher"]

EXPOSE 80



