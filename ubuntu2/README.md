# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t rnjsrnral/ubuntu2:1 .
	docker run -it --rm --name u1  rnjsrnral/ubuntu2:1
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
63a0ba73bf81        rnjsrnral/ubuntu2:1   "/bin/bash"         4 seconds ago       Up 3 seconds                            u1
```

To test,
```
	tree
```
To Rollback
```
    docker rm u1 -f 
    docker rmi rnjsrnral/ubuntu2:1
```
