# Deployment on Ubuntu 17.10
1. Installing docker
2. Downloading the Hortonworks Sandbox
3. Loading sandbox image to docker
4. Starting sandbox
5. Additional info

## 1. Installing docker
1. Check your Ubuntu distribution by `lsb_release -a`
2. Get your package from: https://download.docker.com/linux/ubuntu/dists/ For Ubuntu 17.10, it is under [/pool/edge/amd64/](https://download.docker.com/linux/ubuntu/dists/artful/pool/edge/amd64/)
3. Install package: `sudo dpkg -i <docker_package>.deb`

## 2. Downloading the Hortonworks Sandbox
Get HDP Sandbox for Docker from https://hortonworks.com/downloads/#sandbox

> It is better to use [uGet](http://ugetdm.com/) download manager since the file is ~12Gb: `sudo apt update && sudo apt install uget`

> HDP v2.6.3: https://downloads-hortonworks.akamaized.net/sandbox-hdp-2.6.3/HDP_2.6.3_docker_10_11_2017.tar

## 3. Loading sandbox image to docker

`docker load -i <HDP_sandbox_docker_image>.tar`

## 4. Starting sandbox
1. Get the official `start_sandbox-hdp.sh` script from [HERE](https://raw.githubusercontent.com/hortonworks/data-tutorials/master/tutorials/hdp/sandbox-deployment-and-install-guide/assets/start_sandbox-hdp.sh)
2. Save it as `start_hdp` under `/usr/local/bin/` directory
3. Then make it executable by `sudo chmod +x /usr/local/bin/start_hdp`
4. Start sandbox-hdp container by `sudo start_hdp`
5. Login to ambari server on browser through `127.0.0.1:8080`

## 5. Additional Info
* Load a docker image by `docker load i <docker_image>`
* List loaded docker images `docker images`
* Run docker container by `docker run <docker_image>`
* List running and exited (stopped) docker containers `docker ps -a`
* Stop container by `docker stop <docker_image>`
* Remove container from `ps` by `docker rm <docker_image>`
* Delete docker image by `docker rmi <docker_image>`

### Resources
* Install docker-ce on Ubuntu: https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#install-docker-ce

* Docker CLI commands: https://docs.docker.com/engine/reference/commandline/docker/

* Hortonworks sandbox deployment and install guide: https://hortonworks.com/tutorial/sandbox-deployment-and-install-guide/section/3/

