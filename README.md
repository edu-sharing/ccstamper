# ccstamper

![alt tag](https://github.com/rootzoll/ccstamper/blob/master/static/ccstamper-idee.png?raw=true)

a stateless web service adding creative commons meta data to images 

## Setup Locally (for development)

```
npm install
npm start
```

To run service on local development 'ImageMagick' and 'ExifTool' need to be installed. If you dont can/want to install these edit JS files and build local docker to test run.

## Run from DockerHub

```
docker run -d --name ccstamper -p 3006:3006 rootzoll/ccstamper
docker logs ccstamper -f
```

## Build and Run Docker Locally

```
docker build -t="rootzoll/ccstamper" .
docker run -d --name ccstamper -p 3006:3006 rootzoll/ccstamper
docker logs ccstamper -f
```

## ccstamper API v0.1

Run Docker container locally and open in browser to see API live doc
```
http://localhost:3006
```
