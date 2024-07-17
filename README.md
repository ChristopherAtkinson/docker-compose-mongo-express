> [!IMPORTANT]
> Distributed under the MIT License. See [LICENSE](LICENSE) for more information.

# Docker Compose with Mongo Express

This repository provides a Docker Compose configuration to set up a local environment with MongoDB and Mongo Express. It includes a basic setup with default credentials, allowing for easy development and testing. MongoDB serves as the database, while Mongo Express offers a user-friendly web interface to interact with your MongoDB instance.

## Cloning Repository

```console
$ git clone https://github.com/ChristopherAtkinson/docker-compose-mongo-express.git
```

```console
$ cd docker-compose-mongo-express
```

## Running Development Database

Docker Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration.

```console
$ docker compose up -d

  [+] Running 3/3
   ✔ Network docker-compose-mongo-express_mongo-compose-network  Created
   ✔ Container mongo                                             Healthy
   ✔ Container mongo-express                                     Started
```

> [!NOTE]
> This command does the work of the docker-compose build and docker-compose run commands. It builds the images if they are not located locally and starts the containers. If images are already built, it will fork the container directly.

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.