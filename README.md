# Dockerfile to build a cypress image for Apple silicon M1 Macs

This Dockerfile is inspired by https://github.com/cypress-io/cypress-docker-images/issues/431#issuecomment-1024787781 but stripped down to the bare minium to run Cypress inside Electron.

## Build example
```
docker build -t "cypress/m1:9.3.1" .
```

## Execution example
```
docker run -it -v $PWD:/e2e -w /e2e cypress/m1:9.3.1
```

## Prebuilt on Dockerhub
```
docker pull silvanadrian/cy-m1:9.3.1
```
