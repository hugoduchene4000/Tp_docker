
Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

REPOSITORY    TAG       IMAGE ID       CREATED        SIZE
ubuntu        latest    bf16bdcff9c9   6 days ago     78.1MB
nginx         latest    be69f2940aaf   6 weeks ago    192MB
hello-world   latest    74cc54e27dc4   4 months ago   10.1kB
CONTAINER ID   IMAGE         COMMAND                  CREATED              STATUS                          PORTS                                 NAMES
b8d3a6c67fb8   hello-world   "/hello"                 About a minute ago   Exited (0) About a minute ago                                         elegant_mendeleev
238e3c01935b   nginx         "/docker-entrypoint.…"   16 minutes ago       Up 16 minutes                   0.0.0.0:80->80/tcp, [::]:80->80/tcp   lucid_visvesvaraya
5d4852ad8529   nginx         "/docker-entrypoint.…"   25 minutes ago       Exited (0) 19 minutes ago                                             determined_panini
7e465d266022   ubuntu        "bash"                   27 minutes ago       Exited (130) 27 minutes ago                                           determined_margulis
e7da804fa066   hello-world   "/hello"                 28 minutes ago       Exited (0) 28 minutes ago                                             optimistic_swirles
