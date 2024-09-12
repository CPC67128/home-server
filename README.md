# HomeServer
Home Server Setup

## Ubuntu Server

https://ubuntu.com/download/server

## Portainer

https://docs.portainer.io/start/install-ce/server/docker/linux

```
$ sudo docker volume create portainer_data
$ sudo docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:2.21.1
$ sudo docker ps
```

