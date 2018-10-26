Docker (Very) Basics
--------------------

**Install Docker**


Can't do better than the instructions from the source at `Docker Store <https://store.docker.com>`_ (`Mac <https://store.docker.com/editions/community/docker-ce-desktop-mac>`_) and (`Windows <https://store.docker.com/editions/community/docker-ce-desktop-windows>`_).


**Build your first container**

Make a new directory in which to experiment.

Copy the following into a file named 'Dockerfile' in this directory with the following contents.


::

  FROM alpine:3.7
  CMD ["/bin/sh", "-c" , "while :; do echo 'running'; sleep 60; done"]


Then build the image:


::

  docker build -t 'simplest:latest' .


And run it:


::

  docker run -it 'simplest:latest'


Type '^C' (Control-C) to terminate the container. It will run forever if you don't.


That's it! You've successfully defined, built and run a container.




