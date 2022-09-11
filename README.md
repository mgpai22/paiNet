# PaiNet Custom Ergo TestNet Node

- 45 seconds blocktime


## Prerequisites

Docker and docker compose must be installed. This node program should work on both [Windows](https://docs.docker.com/desktop/windows/install/) \
and [Linux](https://docs.docker.com/engine/install/).

The computer should have about 10 GB of space and 2 GB of RAM.

RAM may be able to be customized if you edit the `-Xmx6G` flag in `docker-compose.yml`

## Setup

```
git clone https://github.com/mgpai22/paiNet
```
```
cd paiNet
```
```
nano ergo.conf
```
- Edit the config file as necessary
  - Defaults are fine
  - Make sure to save the file in nano with `ctrl + o ` then exit with `ctrl + x`
  - After editing do this `docker compose up --force-recreate -d` (if already started) to make sure the changes load



```
docker-compose up -d --build
```

Defaults:
```
localhost:9052 --This is the web address to the ergo node
API Key: hello --This is the api key to unlock the ergo node in the web panel
```