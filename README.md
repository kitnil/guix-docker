``` shell
echo "FROM guix:latest" | docker build --label ru.majordomo.docker.cmd="docker run --volume /opt/guix/rootfs/home:/home --volume /gnu:/gnu --volume /var/guix:/var/guix --privileged --network=host --detach --name guix docker-registry.intr/utils/guix:master" -t "docker-registry.intr/utils/guix:master" -
```
