FROM  UBUNTU:20.04

workdir /usr/src/app

# Shoul've changed the name probably but I was lazy and it doesnt matter. 
COPY hello.sh

RUN apt-get update && apt-get install -y curl

CMD ./hello.sh
