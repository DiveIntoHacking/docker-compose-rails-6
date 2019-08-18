# docker-compose-rails-6

This repository defines docker files(Dockerfile and docker-compose.yml) to create the image. The docker image is published and usable from Docker Hub according to the following commands.

```
$ git clone git@github.com:DiveIntoHacking/docker-compose-rails-6.git
$ cd docker-compose-rails-6
$ docker-compose up
$ docker-compose exec web rake db:create
```

You can see Rails top page on http://localhost:3000/.
