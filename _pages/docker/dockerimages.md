---
layout: default
---
- BASE Image.
- COPY Command
- Expose Ports
- Default Commands
- Building Containers
- Launching New Image

```sh
 FROM nginx:1.11-alpine
 ```
 ```sh
 COPY index.html /usr/share/nginx/html/index.html
 ```
 ```sh
 EXPOSE 80
 ```
 ```sh
 CMD ["nginx", "-g", "daemon off;"]
 ```
 ```sh
 docker build -t mywebserver:latest
 ```
 ```sh
 docker run -d -p 80:80 <image-id|friendly-tag-name>
 ```