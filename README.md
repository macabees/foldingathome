# Folding@Home 
Run Folding@Home in docker container on your local system. 

Note: The WebUI is available on port http://localhost/7396.

## foldingathome (Project Info)
[Website](https://foldingathome.org)

## Docker Hub
[Website](https://hub.docker.com/r/macabees/foldingathome/)

## Build image
`$ docker build -t macabees/foldingathome:latest .`

## Docker Push
`$ docker push -t macabees/foldingathome:latest`

Note: requires `docker login`

## Run image
Usage (Anonymous):

`docker run --rm -it -p7396:7396 macabees/foldingathome:latest --gpu=false --smp=true`

Usage (userName/teamNumber):

`docker run --rm -it -p7396:7396 macabees/foldingathome:latest \
--user=userName --team=teamNumber --gpu=false --smp=true`

## Help
`$ docker run -it --rm macabees/foldingathome --help`

Additional configuration parameters can be passed as command line arguments. 
