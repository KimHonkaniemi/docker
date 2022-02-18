docker build . -t backend && docker run -d -p 8080:8080 backend:latest

docker build . -t frontend && docker run -d -p 5000:5000 frontend:latest

I noticed that the button didnt work when I was using 127.0.0.1:8000. But I decided to change it to localhost instead of ip address and it worked...
