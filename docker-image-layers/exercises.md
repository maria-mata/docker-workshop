Rewrite this Dockerfile to be as efficient as possible:

```dockerfile
FROM node:latest
WORKDIR /app
COPY ./ /app
EXPOSE 80
RUN apt-get -y update && apt-get install -y git vim npm nodejs
RUN npm install
CMD ['npm', 'start']
```

---

In which order would you place the following activities:

* Setting the base image
* Installing system dependencies
* Exposing ports
* Setting a non-root user
* Setting the default command
* Copying application files
* Installing app dependencies
