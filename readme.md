# Gource in a Docker container

This is [Gource](http://gource.io/) (a software version control visualization tool) installed in a Docker container.

## How to use it

Change your current directory to the software project you want to visualize and run:

```
docker run --rm -it -v /tmp/.X11-unix:/tmp/.X11-unix -v $(pwd):/repo --env=DISPLAY gtrafimenkov/gource /repo
```
