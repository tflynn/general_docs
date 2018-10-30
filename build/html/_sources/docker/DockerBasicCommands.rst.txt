Docker Basic Commands
---------------------

**Build and tag an image**


::

	docker build [-t <tag>] <. | Dockerfile>


**Load image into a container and run it**


::

	docker run [-it] image[:tag]


**Load image into a container and run  specified command**


::

	docker run -it image[:tag] <command>


**Get list of all container ids**


::

	docker ps -a


**Delete a (stopped) container**


::

	docker rm <container id>


**Delete every (stopped) container in list**


::


	docker rm $(docker ps -a -q)


**List all image ids**


::


	docker images -q


**Delete all images**


::

	docker rm $(docker images -q)


**Pull an image or a repository from a registry**


::

	docker pull <image[:tag]>


**Push an image or a repository to a registry**


::

	docker tag <image> <repo|registry>

	docker push <image[:tag]>

