# README #

Last tested with node version 6.10.1 and yarn version 0.23.2

## Development mode ##
To install dependencies run
```
$ yarn
```
To start server run
```
$ npm run start
```

## Production mode (mode used on AWS)
Production mode requires docker and docker-compose
To install dependencies run
```
$ yarn
```
Ensure the network is created (only needs to be done once)"
```
$ docker network create sr_network
```
To start server run
```
$ npm run start:prod
```

All external_links (listed in docker-compose.yml) must be fully up before this container can initially run;
eternal_links are allowed to go down and up after this container has started.