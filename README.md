# Platform API

This is a python application (Provider) for explanation of Contract Testing based on [Pact](https://docs.pact.io/).

## Requirements

* `docker >= 20.10.5`
* `docker-compose >= 1.28.5`

## Installing

Run the stack via docker-compose

``` bash
docker-compose --build
docker-compose up -d
```

## Usage

This is a sample Flask application that expose endpoints with REST standard.

|  endpoint      | method   | payload | description |
| ---            | ---      | ---     | ---         |
| /user          | `GET`    | | show all users |
| /user          | `POST`   | `{'name','description'}` | create user |
| /user/**:id**  | `GET`    | | show user with **:id** |
| /user/**:id**  | `DELETE` | | delete user with **:id** |
