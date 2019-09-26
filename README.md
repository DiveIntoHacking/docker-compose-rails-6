# docker-compose-rails-6

This repository defines docker files(Dockerfile and docker-compose.yml) to create the image. The docker image is published and usable from Docker Hub according to the following commands.

```
$ git clone git@github.com:DiveIntoHacking/docker-compose-rails-6.git
$ cd docker-compose-rails-6
$ docker-compose run --rm web bundle install
$ docker-compose run --rm web yarn install
$ docker-compose up
$ docker-compose exec web ./bin/rails db:create
```

You can see Rails top page on http://localhost:3000/.


## pry

If you want to attach a docker process after you stop at a break point with pry, use the following command.

```
$ ./bin/docker-compose-attach web
```

## Build and push an image to Docker Hub

This is just a note for admin (Ham) to push a docker image on https://hub.docker.com/.

See [reference](https://cloud.docker.com/u/diveintohacking/repository/docker/diveintohacking/docker-compose-rails-6/tags).

For instance, you can set like tag=0.0.4 in the following command.

```
$ ./bin/build-and-push-image $tag
```
