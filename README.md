[![Docker Compose Actions Workflow](https://github.com/snakka-hv/mongodb-replicaset-dockercompose/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/snakka-hv/mongodb-replicaset-dockercompose/actions/workflows/main.yml) [![CodeQL](https://github.com/snakka-hv/mongodb-replicaset-dockercompose/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/snakka-hv/mongodb-replicaset-dockercompose/actions/workflows/codeql-analysis.yml)

### Pre-requisite
- Docker
- Docker Compose

### Scripts use
- MongoDB Replica Sets
- Mongoose
- Mongoose Transactions

### What this repo does?
Executing the docker compose file will bring up a 3 node mongodb cluster and will
apply the needed replicaSet configurations

If you would like to reduce the number of nodes (for lowering resources consumed etc..)
do modify docker-compose.yml and also scripts/setup.sh accordingly

### Executing
Open ##.env## file and provide a local folder where mongo can store its data. By default
it will create a folder called mongo in the current directory and will use it as
storage volume

Run docker compose file by
- docker-compose up -d

Wait for the nodes to spool up and the cluster should be ready to use

### Shutting down
- docker-compose down


### Credits:
Based on https://gist.github.com/asoorm
