# WIP
This repo is currently work in progress.<br>
Known Bugs:
* haproxy redirects from http://127.0.0.1:1080/index.html to http:///index.html instead of http://docker-ip/index.html
* `Dockerfile` not cleaned up

# docker-farming-simulator-server
This is a docker image to run the Farming Simulator 19 in a docker container.
The game files are **not** included and must be mounted into the container.
The `data` directory should filled with the game binary files and the `save` directory is for the game data files.<br>
Thanks to (cbeneke/docker-farming-simulator-server)[https://github.com/cbeneke/docker-farming-simulator-server] for his work on this docker image.

## Build
`docker-compose build`

## Run
`docker-compose -d up`

## Configuration
The configuration for the docker-container is stored in the `config` directory.
The configuration for the dedicated server is stored in the `data` directory.
The configuration for the game is stored in the `save` directory.
