docker-rstudio-server
=====================

Docker image that runs an rstudio server based on R 3.1.1. This docker image is based on [this rstudio-server docker](https://registry.hub.docker.com/u/mgymrek/docker-rstudio-server). I use this image as a base for other images to provide reproducible and interactive R analyses.

To run:
```
docker run -d -p 49000:8787 wieling/docker-rstudio-server /bin/bash
```
(You can use any open port besides 49000 if you want.)

Then navigate to ```http://0.0.0.0:49000``` or ```http://192.168.59.103:49000``` (login / pass: guest / guest). 