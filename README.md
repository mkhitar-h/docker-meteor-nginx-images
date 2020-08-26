# USE this repo to deploy previously pushed docker image into server

This repo is based templete for Meteor-Mongo-Ngnix setup

Pre-requirements:

The Meteor docker image should be already push in the current repo (to see more: https://github.com/mkhitar-h/docker-meteor-nginx-development-build/blob/master/README.md)

1. Edit docker-compose.yml and change following row:
```
image: docker.pkg.github.com/mkhitar-h/docker-meteor-nginx-images/kerpak:0.0.3
```
To have corresponding image and version.

2. Run following:
```
docker-compose up --build -d
```


Advanced usage:
You can change nginx/nginx.conf to have you own setup for nginx server.
Also feel free to change docker-compose.yml (e.x: adding certs folder, logs folder, etc.)
