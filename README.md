# docker-helloworld

![Docker Pulls](https://img.shields.io/docker/pulls/ddepaoli3/helloworld.svg) ![Automated Builds](https://img.shields.io/docker/automated/ddepaoli3/helloworld.svg) ![Build Status](https://img.shields.io/docker/build/ddepaoli3/helloworld.svg )

A simple helloworld app for docker

A simple nginx helloworld application that helps you learn docker image pulls. Runs on port :80

To pull this image:
```
docker pull ddepaoli3/helloworld
```

To run this image:
```
docker run -p 80:80/tcp "ddepaoli3/helloworld"
```

To build this dockerfile
```
docker build --rm --tag ddepaoli3/helloworld .
```

To push this image to dockerhub
```
docker login --username=ddepaoli3
docker push
```

To push this image to AWS ECR
```
docker tag ddepaoli3/helloworld <aws_account_id>.dkr.ecr.<region>.amazonaws.com/helloworld
aws ecr get-login --profile profilename --region eu-central-1 #then execute the output command
docker push
```

Dockerhub link: https://hub.docker.com/repository/docker/ddepaoli3/helloworld/general

Github link: https://github.com/ddepaoli3/docker-helloworld
