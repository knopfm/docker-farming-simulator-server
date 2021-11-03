This repo is currently work in progress.<br>
Known Bugs:
* haproxy redirects from http://<span></span>127.0.0.1:1080/index.html to http://<span></span>/index.html instead of http://<span></span>docker-ip/index.html
* `Dockerfile` not cleaned up

# docker-farming-simulator-server
This is a docker image to run the Farming Simulator 19 in a docker container.
The game files are **not** included and must be mounted into the container.
The `data` directory should filled with the game binary files and the `save` directory is for the game data files.<br>
Thanks to [cbeneke/docker-farming-simulator-server](https://github.com/cbeneke/docker-farming-simulator-server) for his work on this docker image.

## Build and Run
```bash
# Build
docker-compose build

# Run detached
docker-compose up --detach

# Stop
docker-compose down

# Build and Run
docker-compose up --build
```

## Configuration
The configuration files for the docker-container are stored in the `config` directory.
The configuration files for the dedicated-server are stored in the `data` directory.
The configuration files for the game are stored in the `save` directory.
