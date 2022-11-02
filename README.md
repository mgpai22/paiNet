# PaiNet Custom Ergo TestNet Node

This has been adopted by the ErgoPlatform as the offical testnet

- 45 seconds blocktime

- offical node: http://213.239.193.208:9052/panel
- offical explorer: https://testnet.ergoplatform.com/
- offical api: https://api-testnet.ergoplatform.com/api/v1/docs/
- offical gql: https://gql-testnet.ergoplatform.com/


### down for maintenance 
- live node: https://pai-net.mempoolnode.live/panel
- explorer: https://explorer.mempoolnode.live/
- api: https://api.mempoolnode.live/api/v1/docs/
- gql: https://gql.mempoolnode.live/
- faucet: https://painet-faucet.mempoolnode.live/


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
