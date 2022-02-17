FROM ubuntu:16.04



WORKDIR /usr/src/frontend



COPY . .



RUN apt-get update && apt-get install -y git curl



RUN curl -sL https://deb.nodesource.com/setup_16.x | bash



RUN git clone https://github.com/docker-hy/material-applications.git



RUN apt-get install -y nodejs



RUN npm install -y



RUN npm run build



RUN npm install -g serve



CMD ["serve", "-s", "-l", "5000", "build"]

## there was many errors during the build process but the app works so I don't complain
