Openshift:
it is part of PAAS, and hybrid cluod.

Docker:

> docker search ubuntu

Ubuntu cmd line interface:
> docker run -it ubuntu
cent os install
> apt-get update

running contianer
> docker ps

DockerHub username: yernibabukommoju123

searching for images from neoisone docker id
> docker search neoisone

Openshift:

POD : sandbox with multiple container

kubernetese to find pods

> kubectl get pods

openshift internal projects:

> kubctl get projects

openshift is toplayer on kubernetes.
represent using cmd : oc

>oc get projects

open shift status
> oc status

Docker registery:

RedHat registery:
imgs are pushed to

cmd to find centos ip:
> ip a

connect to centos from local system:
>ssh

To know available softwares

> REPO -repository

installing docker repository in centos:
https://docs.docker.com/install/linux/docker-ce/centos/

Install using the repository

Before you install Docker CE for the first time on a new host machine, you need to set up the Docker repository. Afterward, you can install and update Docker from the repository.
Set up the repository

    Install required packages. yum-utils provides the yum-config-manager utility, and device-mapper-persistent-data and lvm2 are required by the devicemapper storage driver.

    $ sudo yum install -y yum-utils \
      device-mapper-persistent-data \
      lvm2

    Use the following command to set up the stable repository.

    $ sudo yum-config-manager \
        --add-repo \
        https://download.docker.com/linux/centos/docker-ce.repo

$ sudo yum-config-manager --enable docker-ce-nightly

$ sudo yum install docker-ce docker-ce-cli containerd.io

find redhat version:
[root@localhost ~]# cat /etc/redhat-release

CentOS Linux release 7.6.1810 (Core)

To start the docker service cmd:
> systemctl start docker

To find images in docker:
> docker search ubuntu

Installing ubuntu container:
> docker run -it docker.io/ubuntu

To verify:
> cat /etc/os-release

from ubuntu to check whether it is connected to ubuntu or not:
> apt-get update

To check the available containers cmd:
> docker container ls

cmd help:
> docker container cf

How does docker is working?
-> it works on kernell namespace


