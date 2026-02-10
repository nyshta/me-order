Symfony, API Platform, Docker, Sagas with Ecotone, AI planning, Swoole

1. Docker installation:

+ install docker desktop
+ download symfony-docker https://github.com/dunglas/symfony-docker
+ get copilot

2. Services:

FTGO with Symfony:
- Order service
  + put symfony-docker inside the repo
  + install symfony skeleton
  + install db https://github.com/dunglas/symfony-docker/blob/main/docs/mysql.md
  - add db creds to .env from compose.yaml, use AI plan with prompt:
    ````
    put database envs from compose.yaml into .env.dev, .env, .env.example
    ````
  + add makefile 

  - API Platform: first api-endpoint for Order service /order/create
  - Ecotone +stubs for other services
  - Docker: make shared network to make services call each other


- Consumer service
- Kitchen service
- Accounting service

3. Network
- docker network to make it work all together

4. Saga:
- CreateOrderSaga with Ecotone

5. Swoole:
- create alternative Order Service with Swoole


-----------
DOCKER
- compose.yaml vs compose.override.yaml vs compose.prod.yaml
- networks
- images and instances
- ports
- volumes
- entrypoint
