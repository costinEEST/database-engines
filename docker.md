- When you spin up a docker container named `pg` for example, you can connect to it that in two methods

1) Expose the port to your host machine as I do in all the examples in this course. E.g  For example if I run my container with the option `-p 5555:80` this exposes port 80 in the container to your host machine. For instance, my host machine is `husseinmac`, I can access the container using `husseinmac:5555`

2) Access the docker container IP directly. This doesn't work on mac but works on other operating systems. You can do `docker inspect pg` to reveal the IP address of the container then connect to it. e.g. `172.17.0.3:80` or `172.17.0.3:5432`
