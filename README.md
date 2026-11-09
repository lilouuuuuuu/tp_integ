# tp_integ
TP pour intégration et déploiement continus


# Exercice : Manipulation de base des conteneurs

1. docker --version
    
    Docker version 29.9.2, build a82e528

2. docker images

    IMAGE   ID             DISK USAGE   CONTENT SIZE   EXTRA

3. docker pull hello-world

    Using default tag: latest
    latest: Pulling from library/hello-world
    4f55086f7dd0: Pull complete 
    d5e71e642bf5: Download complete 
    Digest: sha256:c567b231f65614688711a75f31518a064258a51d442117a3e771a3a8fdba78ef
    Status: Downloaded newer image for hello-world:latest
    docker.io/library/hello-world:latest

4. docker run hello-world

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


5. docker ps 

    CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES

6. docker ps -a

    CONTAINER ID   IMAGE         COMMAND    CREATED              STATUS                          PORTS     NAMES
    bf08f1ec6d40   hello-world   "/hello"   About a minute ago   Exited (0) About a minute ago             condescending_euler

7. docker rm bf08f1ec6d40
    
    bf08f1ec6d40

8. a. docker images
    
    hello-world:latest   c567b231f656       25.9kB         9.49kB        

    b. docker rmi c567b231f656

    Untagged: hello-world:latest

    Deleted: 
    sha256:c567b231f65614688711a75f31518a064258a51d442117a3e771a3a8fdba78ef

