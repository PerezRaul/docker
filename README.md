# Requirements

- [Docker](https://www.docker.com/products/docker-desktop)

# Installation

Clone this repository on _~/Sites_ with _docker_ name and follow this instructions:

---

1 - Copy the .env.example file:
```shell
> cd ~/Sites/docker
> cp .env.example .env
```

---

2 - Build containers and start with the following commands:

```shell
> docker compose build nginx php-fpm docker-in-docker workspace
> docker compose up nginx php-fpm docker-in-docker workspace
```

---

# Working

All you need in order to install composer dependencies or what else the project need is enter on the workspace container with that command:

---

```shell
> docker compose exec workspace bash
```
