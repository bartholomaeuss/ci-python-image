# CI PYTHON IMAGE

### Prerequisite

```bash
./hello_world.sh
```

### Windows

```bash
./provide_container.sh
```

### More

```
sudo docker run -d --net=host --restart=unless-stopped releases-docker.jfrog.io/jfrog/artifactory-jcr:latest
```

#### Login into Docker artifactory using docker cli

```
echo "<password>" | docker login -u <user> --password-stdin <host>:8082/docker
```

#### Push given docker image manually into local artifactory


```
docker tag ci-python:3.13-slim <host>:8082/docker-dev/ci/python/amd64:latest
```
```
 docker push <host>:8082/docker-dev/ci/python/amd64:latest
```

See the official
[python artifactory](https://)
documentation.
See also the official
[installation manual](https://).
See also the official
[artifacts](https://)