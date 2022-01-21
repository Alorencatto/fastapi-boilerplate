# Template FastAPI com Postgres, Uvicorn, and Traefik


### Development

Realizando o build dos containers:

```sh
$ docker-compose up -d --build
```

Urls para teste:

1. [http://fastapi.localhost:8008/](http://fastapi.localhost:8008/)
1. [http://fastapi.localhost:8081/](http://fastapi.localhost:8081/)

### Produção

Deve-se mudar o domínio no arquivos *docker-compose.prod.yml*, adicionando o email no *traefik.prod.toml*.

Realizando o build dos containers:

```sh
$ docker-compose -f docker-compose.prod.yml up -d --build
```
