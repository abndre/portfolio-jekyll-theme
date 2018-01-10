---
layout: post
title: "Hello Docker"
---

Virtualização, Não. Docker. Usa-se os serviços da máquina hospedeiro. Ganho em velocidade.

Enfim vamos lá.

# 1. Instale o Docker no seu sistema.

```bash
$ sudo docker ps
$ sudo docker image
```

Não terá imagem e nenhuma sistema rodando. Vamos criar um.

```bash
$ sudo docker run -it ubuntu:16.04 /bin/bash
```

## -it para rodar um serviço
## /bin/bash para ter um terminal

```bash
$ sudo docker run -it -p 8080:80 ubuntu:16.04 /bin/bash
```

## 8080:80 agora tem uma porta rodando

Para sair da maquina CTRL + Q + P e para voltar faça docker ps para verificar as imagens e depois

```bash
$ sudo docker ps
$ sudo docker attach <CONTAINER ID>
```
