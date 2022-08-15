# docker-samples
A set of Docker configuration for a variety of Data Science projects

## Jupyter

This is a starter image with Python 3.9.13 and Jupyter notebook. 

See [jupyter](./jupyter/) for more details.

## Postgres SQL and Metabase

It is a Docker compose running three containers: 
- [Metabase](https://www.metabase.com/docs/latest/operations-guide/running-metabase-on-docker.html#use-docker-secrets-to-hide-sensitive-parameters)
- [Postgres 12](https://github.com/docker-library/docs/blob/master/postgres/README.md)  as a storage for Metabase
- [Adminer](https://www.adminer.org) as a DB management tool.

