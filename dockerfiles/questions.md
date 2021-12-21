* How many `FROM` statements can a Dockerfile have? Why?
A Dockerfile can have multiple `FROM` statements to create multiple images or use one build stage as a dependency for another. There is no limit to the number of `FROM` statements in a Dockerfile.
* What language are `RUN` commands in Dockerfiles written in?
Bash
* Does `EXPOSE` makes a port available on the host? Why or why not?
`EXPOSE` is used to make a port available in the container to the host.
* What's the difference between `ENTRYPOINT` and `CMD`?
`ENTRYPOINT` is meant to not be overridden.
* What happens when the value in a Dockerfile and the value in a Docker Compose file conflict?
The following values in a Dockerfile cannot be overridden: FROM, MAINTAINER, RUN, and ADD. All others can be overridden at runtime, which means the Docker compose file would override all other values in the Dockerfile if a conflict exists.
* What is the purpose of `ENV` variables in Dockerfiles?
To set environment variables that need to be available to subsequent instructions in the build stage.
