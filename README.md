# Imageboard-server

This is the backend server to be used with imageboard-web. It is intended to be
a classic image-board website clone.

## Installation

### Dependencies

- dotnet-sdk 3.1
- docker
- docker-compose

### How to use

First, you must copy the provided `.env-sample` file to create a new `.env`
file. This file contains environment-dependant configurations, such as database
connections, hosts, api-keys etc.

Then, in a terminal, you can use `docker-compose up` to start the Postgresql database.

In a second terminal, you can use `dotnet restore` to install all packages
specified in the `imageboard-server.csproj` file.

When the installation is over, you can use `dotnet watch run` to start the server with
hot-reloading. Whenever you change a file in imageboard-server, the server will
restart (Might have to wait a second or two)

