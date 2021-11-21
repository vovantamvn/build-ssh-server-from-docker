# build-ssh-server-from-docker

Build ssh sever from Docker.

## Usage

### Build image

```sh
docker build -t ssh_server .
```

### Run a container

```sh
docker run --name ssh_server -p 8000:22 -d -it ssh_server
```

### SSH to container

```sh
ssh -p 8000 root@localhost -i ./id_rsa
```

You can use ssh-keygen to replace the key above.
