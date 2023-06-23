## jupyker
jupyker: jupyter notebooks packaged in docker container. Cute, eh?

#### First, docker commands:

##### bring up container

```docker-compose up```

##### shut down container

```docker-compose down```

##### view reclaimable memory

```docker system df```

##### clean up total reclaimable size for images, network, volume

```docker system prune -a```

#### Installing Docker on Ubuntu

```https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04```

```sudo apt update```

```sudo apt install apt-transport-https ca-certificates curl software-properties-common```

```curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -```

```sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"```

```apt-cache policy docker-ce```

```sudo apt install docker-ce```

```sudo systemctl status docker```

##### docker system file

```/lib/systemd/system/docker.service```

#### docker daily commands

```sudo systemctl status docker```

```sudo systemctl start docker```

```sudo systemctl stop docker```

###### options for starting docker daemon

```sudo /usr/bin/dockerd --help```

#### jupyter commands:

```https://localhost:8888/jupyter/minimal-notebook```
-----------------------

### TROUBLESHOOTING

**PROBLEM:** Out of memory errors when you run docker-compose up

**SOLUTION:** May need a newer version of Docker or allocate more memory




