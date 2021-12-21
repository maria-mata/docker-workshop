* Dockerfile
A file containing instructions for how to build a Docker image.
* Docker Image
A compiled Dockerfile
* Dockerfile: FROM
Defines what Docker image the container should be based on.
* Dockerfile: WORKDIR
The current working directory.
* Dockerfile: COPY
Copy files from the host computer to the container.
* Dockerfile: RUN
Executes a shell command inside of the container.
* Dockerfile: ENV
Defines environment variables
* Dockerfile: EXPOSE
Expose a port inside the container
* Dockerfile: ENTRYPOINT
Define a command that should run whenever a container is created with this image. Should not be overridden.
* Dockerfile: CMD
Define a command that should be run instead of ENTRYPOINT - OR - define the arguments or options to an ENTRYPOINT
* Clobber
??
