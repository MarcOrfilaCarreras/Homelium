<!-- Top -->

<div id="#top"></div>

<h1 align="center">Homelium</h1>

<div align="center" >

[![License](https://img.shields.io/github/license/MarcOrfilaCarreras/Homelium?style=for-the-badge)](https://github.com/MarcOrfilaCarreras/Homelium) [![Last Commit](https://img.shields.io/github/last-commit/MarcOrfilaCarreras/Homelium?style=for-the-badge)](https://github.com/MarcOrfilaCarreras/Homelium) [![Stars](https://img.shields.io/github/stars/MarcOrfilaCarreras/Homelium?style=for-the-badge)](https://github.com/MarcOrfilaCarreras/Homelium)

</div>

<!-- Content -->

## Getting Started

> This design is inspired by [Walkx](https://github.com/WalkxCode).

### Installation

The best way to install this software is using Docker.

First, download the image from the Github repository.

```
docker pull ghcr.io/marcorfilacarreras/homelium:amd64
```

Then run it with the following command.

```
docker run -d -p 5000:5000 -v ${PWD}/config.json:/app/app/config.json:rw ghcr.io/marcorfilacarreras/homelium:amd64
```

You can also use a **docker-compose.yml**.
```
version: "3.7"

services:
  homelium:
    container_name: Homelium
    image: ghcr.io/marcorfilacarreras/homelium:amd64
    ports:
      - 8000:5000
    volumes:
      - ${PWD}/config.json:/app/app/config.json:rw
```

You will have to create a file called **config.json** with the following content:
```
[]
```

## License

Distributed under the MIT License. See `LICENSE` for more information.