## Run below command to pull jenkins image and then run as container.
### 1. Build a new docker image from this Dockerfile :

```bash 
docker build -t nginx:webserver .
```
```bash 
docker run --name nginx-webserver -d -p 8067:80 nginx:webserver
docker run --name nginx-webserver -d -p 8067:80 -v ${PWD}/nginx:/etc/nginx/  -v ${PWD}/www:/usr/share/nginx/ nginx:webserver
```
