# jupyker
jupyker: jupyter notebooks packaged in docker container. Cute, eh?

First, docker commands:
bring up container
{{{docker-compose up}}}
#shut down container
docker-compose down
#view reclaimable memory
docker system df
#clean up total reclaimable size for images, network, volume
docker system prune -a

#Installing Docker on Ubuntu
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04
#docker system file
/lib/systemd/system/docker.service

#example commands
sudo systemctl status docker
sudo systemctl start docker
sudo systemctl stop docker
#options for starting docker daemon
sudo /usr/bin/dockerd --help
-----
TROUBLESHOOTING

PROBLEM: Out of memory errors when you run docker-compose up
SOLUTION: May need a newer version of Docker or allocate more memory

#Once container is running, some jupyter commands to work with it:

