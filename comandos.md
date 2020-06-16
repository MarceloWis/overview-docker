# Comandos Básicos

## docker run
```bash
> docker run -it ubuntu /bin/bash
```

**-it**: Terminal Interativo

## docker ps
Listagem de containers rodando

## docker ps -a
Lista todos os container mesmo os que estão parados

## docker run -d
`-d`: detached

Vai deixar o processo da imagem rodando com o terminal livre
```bash
docker run -d nginx
```
## docker run -p 8080:80
`-p`: Port

Libera a porta 8080 na sua máquina local e é redirecionado para a porta 80 do container
```bash
docker run -d -p 8080:80 nginx
```

## docker rm
Remover um container que não está rodando.

```bash
> docker rm id
```
Mata o processo do container e apaga
```bash
> docker rm id -f
```
Apaga tudo sobre a imagem na maquina
```bash
> docker rmi {name}
```


## docker exec
Entrar no container

```bash
> docker exec -it {id} bash
```

Tudo que for editado na imagem será perdido quando o container parar.

## docker images
Imagens do cache da sua máquina.

