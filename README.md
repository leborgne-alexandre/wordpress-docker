# wordpress

## Installation

```console
$ git clone https://github.com/aminnairi/wordpress-docker.git ~/code/my-wordpress-app
$ cd ~/code/my-wordpress-app
```

Where `~/code/my-wordpress-app` is the path to where you want to have your Wordpress website.

## Start

```console
$ make start
```

***Note**: the server will be accessible on http://localhost:8080. If you want to use a different port, change it in the [`.env`](./env) file.*

## Stop

```console
$ make stop
```

## Restart

```console
$ make restart
```

## Update

```console
$ make update
```

***Note**: this will update the Docker configurations by fetching newer versions of this repository from GitHub. This will not touch any files under the `database` or `server` folders.*

## Architecture

Folder | Description
---|---
`database` | MySQL related files for persistence.
`docker/database` | MySQL Docker configuration.
`docker/server` | Wordpress Docker configuration.
`server` | Wordpress source files.