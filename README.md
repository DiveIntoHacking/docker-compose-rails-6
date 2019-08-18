# docker-compose-rails-6

This repository defines docker files(Dockerfile and docker-compose.yml) to create the image. The docker image is published and usable from Docker Hub according to the following commands.

```
$ git clone git@github.com:DiveIntoHacking/docker-compose-rails-6.git
$ cd docker-compose-rails-6
$ docker-compose up
$ docker-compose exec web rake db:create
```

You can see Rails top page on http://localhost:3000/.

## build and push to Docker Hub

This is just a note for admin to push a docker image on https://hub.docker.com/.

```
$ docker-compose -f docker-compose.build.yml build --no-cache
$ docker push diveintohacking/docker-compose-rails-6:tag
```
