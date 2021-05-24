## This a very simple project to show how to build a docker image with nodeJs

### Docker - build image

The docker build command reads the Dockerfile and executes its content.

> docker build -t node-hello-world-image . 

### Docker run container

With this command we run a container using the image on port 3000

> docker run -d -p 3000:3000 --name node-app node-hello-world-image

```
$ docker ps
CONTAINER ID   IMAGE                    COMMAND                  CREATED         STATUS         PORTS                    NAMES
74ee1bf096c9   node-hello-world-image   "docker-entrypoint.s…"   9 seconds ago   Up 7 seconds   0.0.0.0:3000->3000/tcp   node-app
```

Go to  http://localhost:3000
