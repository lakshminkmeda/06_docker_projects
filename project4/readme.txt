Simple Hello World app for Docker testing

1. The hello world app uses nodejs and listens on port 3000. The output is a simple "Hello Node" message.

Useful commands:


docker build -t myapp:v1 .
docker run -d -p 3000:3000 myapp:v1
