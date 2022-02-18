FROM golang:1.16



WORKDIR /usr/src/backend



COPY . .



RUN apt-get update && apt-get install -y git curl



RUN curl -sL https://deb.nodesource.com/setup_16.x | bash



RUN git clone https://github.com/docker-hy/material-applications.git



RUN apt install -y nodejs



RUN go build





CMD ["./server"]

