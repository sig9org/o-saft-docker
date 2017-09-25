# O-Saft Docker Container

This repository contains a Docker container for the [OWASP SSL advanced forensic tool](https://github.com/OWASP/O-Saft).

## Usage

    docker run sig9/docker-o-saft +check www.nicksays.co.uk

## Development

The container is configured an entrypoint of `perl /opt/osaft/o-saft.pl`.  If you want to jump into the container then you'll need to override the entrypoint at runtime using `--entrypoint`, for example:

    $ docker run -it --entrypoint=bash sig9/docker-o-saft
    root@2791d357b433:/opt/osaft#

## See also:

- [punkstar/docker-o-saft - GitHub](https://github.com/punkstar/docker-o-saft)
- [punkstar/o-saft - DockerHub](https://hub.docker.com/r/punkstar/o-saft/)

