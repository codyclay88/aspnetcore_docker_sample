This is a sample app which explains how to use Docker in the development phase of an application.

For container to scaffold project within container
```
docker run --rm -it -p 5000:5000 -p 5001:5001 -v $(pwd -W)/web-api:/app mcr.microsoft.com/dotnet/core/sdk:2.2-stretch bash
```

For running container from our Dockerfile
```
docker run --rm -it -p 5000:5000 -p 5001:5001 --name sample-web-api sample-web-api
```