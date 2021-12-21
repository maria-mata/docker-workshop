* Describe image layers in your own words.
Images have many layers. A new layer gets created with each `RUN`, `ADD`, and `COPY` command, and these layers are stacked in the final image that is created.
* Why is it useful to combine `RUN` commands with `&&`?
Each `RUN` instruction creates a new image layer, so combining multiple commands into the same `RUN` reduces the number of extra image layers that are created.
* How should Docker layers generally be ordered?
From least changing to most changing.
* Why is it useful to split up `COPY` commands?
Because some files can change a lot, so splitting into separate `COPY`'s ensures that if a particular file changes only the corresponding image layer needs to be rebuilt.
* Differentiate between Linux images designed for Docker vs. desktop Linux.
Linux images designed for Docker are generally more lightweight, as they only include the dependencies needed to run the specific application that is supported by that image. By contrast, images designed for desktop have a lot more dependencies and things as they are meant to support multiple different programs on the host computer.
* Why would something go in a `.dockerignore` file?
To ensure it doesn't get added to or used by the docker image.
