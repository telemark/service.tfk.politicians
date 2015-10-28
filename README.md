# service.tfk.politicians
docker-compose file for the politicians service in Telemark County Council

## Docker

Start containers via docker-compose

```sh
$ docker-compose up
```

## Setup mongodb indexes

```sh
$ mongo 192.168.99.100:27017/tfk config/mongodb.indexes
```

## Import data

```sh
$ mongoimport -h 192.168.99.100:27017 -d tfk -c politicians data/politicians.json --jsonArray
```

