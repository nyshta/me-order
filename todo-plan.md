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
  - add mysql creds to .env from compose.yaml, use AI plan with prompt:
    ````
    put database envs from compose.yaml into .env.dev, .env, .env.example
    ````
  - add makefile 
- Consumer service
- Kitchen service
- Accounting service

3. Network
- docker network to make it work all together

4. Saga:
- CreateOrderSaga with Ecotone

5. Swoole:
- create alternative Order Service with Swoole
