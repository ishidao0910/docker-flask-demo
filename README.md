# docker-flask-demo
hands on for me to create docker environment.

# select OS
```
docker pull ubuntu:latest
```

# write dockerfile
```Dockerfile
FROM ubuntu:latest

RUN apt-get update
RUN apt-get install python3 python3-pip -y

RUN pip3 install flask
```

# build
```
docker build . -t test/hoge:1.0
```

# docker run and container login
```
docker run -it hoge/fuga:1.0 /bin/bash
```

# python login
```
python3
```

# login container again
```
docker exec -it {{conteiner name}} /bin/bash
```

# delete container
```
docker rm {{container name}}
```
