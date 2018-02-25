---
layout: default
---
```sh
FROM nginx:alpine
COPY . /usr/share/nginx/html  
```
Build Docker Image 
```sh
docker build -t <build-directory>  -t tag 
```
```sh
docker build -t webserver-image:v1 .
```
Run The Image
```  
-p <host-port>:<container-port>.
```

```sh 
docker run -d -p 80:80 webserver-image:v1
```