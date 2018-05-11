# Docker - ThrustJS [![Build Status](https://travis-ci.org/Thrustjs/thrust-docker.svg?branch=master)](https://travis-ci.org/Thrustjs/thrust-docker)

Este repositório contém a receita oficial do Docker para a plataforma ThurstJS.

## Build

```bash
docker build -t thrust .
```

## Uso

```bash
docker run --rm -it -v $(pwd):/app -w /app thrust /bin/sh -c "thrust install && thrust startup.js"
```

## Exemplo

### Comandos:
```bash
mkdir exemplo
cd exemplo
echo "print('Ola Mundo\!')" > main.js
docker run --rm -it -v $(pwd):/app -w /app thrust /bin/sh -c "thrust main.js"
```
### Saída:
```bash
Ola Mundo!
```