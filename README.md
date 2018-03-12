``` bash
##########################################################################
#  _     _                     __     __             ____                #
# | |   | | __ _ _ __ ___   __ \ \   / /_ _ _ __    / ___|___  _ __ ___  #
# | |   | |/ _` | '_ ` _ \ / _` \ \ / / _` | '_ \  | |   / _ \| '__/ _ \ #
# | |___| | (_| | | | | | | (_| |\ V / (_| | | | | | |__| (_) | | |  __/ #
# |_____|_|\__,_|_| |_| |_|\__,_| \_/ \__,_|_| |_|  \____\___/|_|  \___| #
#                                                                        #
##########################################################################
```

## Build Status
[![Build status](https://travis-ci.org/Nanielito/llamaVanCore.svg?master)](https://travis-ci.org/Nanielito)

## Pre-requisites
* MongoDB
* Node.js
* Git 

## Setup

### Install dependencies

#### MongoDB
Go to MongoDB main page (https://www.mongodb.com/), download and install.

### Node.js
Go to Node.js main page (https://nodejs.org/en/), download and install.

### Git
Go to Git main page (https://git-scm.com/), download and install.

#### To get source code from parent repository
``` bash
> $ git clone https://github.com/nanielito/llamaVanCore.git
```

### To install Node.js dependencies
``` bash
> $ npm install
```

### Docker (Alternative)
Docker can be used as an alternative to create instances for database and application core.

Go to Docker main page (https://www.docker.com), install docker engine and docker compose. 

## Development

### To start MongoDB server:         
``` bash
> $ mongod
```

### To create the MongoDB docker container (Alternative):
``` bash
> cd docker
> docker-compose up -d llamavandb
```

### To create the application docker container (Alternative):
``` bash
> cd docker
> docker-compose up -d llamavancore
```

### To create the application docker container for a development environment (Alternative):
``` bash
> cd docker
> docker-compose up -d llamavancore-dev
```

### To start, restart and stop docker containers:
``` bash
> docker-compose start CONTAINER
> docker-compose restart CONTAINER
> docker-compose stop CONTAINER
```
Go to Docker Compose page documentation (https://docs.docker.com/compose) to view more details.

* ##### You can use [DockerUtils](https://nanielito.github.io/DockerUtils/) library as a middleware to handle docker-compose commands.

### To start the Node.js server: 
``` bash
> $ npm start
```

### To start the Node.js server in development: 
``` bash
> $ npm start:dev
```

### To preview the app on web browser
Go to http://localhost:3000

## Git Rules

### Commit messages:
Use the following prefix to classified the actions made:
* #N for adding new features.
* #M for updating features.
* #R for removing features or some piece of code.
* #F for fixing some bug on features.

### Branches
Use the following prefix to create branches:
* feature/FUNCTIONALITY-NAME for normal development.
* fix/ISSUE-DESCRIPTION for bug's fix.

## Version
v0.1.0

## Author
* **DER** - *Initial work* - [nanielito](https://github.com/nanielito)
* **EYT** - *Contributor* - [enriqueyt](https://github.com/enriqueyt)
* **JPI** - *Contributor* - [pitajuan](https://github.com/pitajuan)
* **DMA** - *Contributor* - [deyvidm18](https://github.com/deyvidm18)

## Licence
ISC

