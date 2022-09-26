# setup wso2


## build an image of your express app

- my repo is at https://github.com/tobecci/wso2Test (you can use yours of course)
- run the command below to build the image of your express app

```bash
docker build -t tobecci/express:1.0.0 .
```
- replace `tobecci/express:1.0.0` with whatever you want, but take note of it, because you will add it to the docker compose config
- open `docker-compose.yaml`, replace `tobecci/express:1.0.0` with the image name you chose

> MAC USERS: replace `image: wso2/wso2am:4.1.0-alpine` with the right docker image for you
- run `docker compose up` to start it
- the url to use for the endpoint is `http://node-app:5000/` your port might be different

## Accessing management console

visit the following URLs

| Name                         | URL                              |
| ---------------------------- | -------------------------------- |
| Carbon Management Console    | https://localhost:9443/carbon    |
| API Manager Publisher        | https://localhost:9443/publisher |
| API Manager Developer Portal | https://localhost:9443/devportal |
