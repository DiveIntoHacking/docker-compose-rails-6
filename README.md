# docker-compose-rails-6

This repository defines docker files(Dockerfile and docker-compose.yml) to create the image. The docker image is published and usable from Docker Hub according to the following commands.

```
$ git clone git@github.com:DiveIntoHacking/docker-compose-rails-6.git
$ cd docker-compose-rails-6
$ docker-compose up
$ docker-compose exec web rake db:create
```

You can see Rails top page on http://localhost:3000/.

## Build and push an image to Docker Hub

This is just a note for admin (Ham) to push a docker image on https://hub.docker.com/.

See [reference](https://cloud.docker.com/u/diveintohacking/repository/docker/diveintohacking/docker-compose-rails-6/tags).

```
$ docker-compose -f docker-compose.build.yml build --no-cache
```

```
$ docker images
REPOSITORY                   TAG                 IMAGE ID            CREATED              SIZE
docker-compose-rails-6_web   latest              3614c5a22c6c        About a minute ago   1.39GB
```


```
$ docker tag docker-compose-rails-6_web:latest diveintohacking/docker-compose-rails-6:0.0.1
```



```
$ docker push diveintohacking/docker-compose-rails-6:0.0.1
```
