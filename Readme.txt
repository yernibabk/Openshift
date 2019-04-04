Docker:
Docker is a container management service.

Docker Engine − It is used for building Docker images and creating Docker containers.

Docker Hub − This is the registry which is used to host various Docker images.

Docker Compose − This is used to define applications using multiple Docker containers.

In Docker, everything is based on Images. An image is a combination of a file system and parameters.

> docker run hello-world 

    The Docker command is specific and tells the Docker program on the Operating System that something needs to be done.

    The run command is used to mention that we want to create an instance of an image, which is then called a container.

    Finally, "hello-world" represents the image from which the container is made.


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

To connect container from localhost:
> docker run -it ubuntu

To run container in background:
[root@localhost ~]# docker run -it -d ubuntu
6e0697841ff5ac51df6b1f6550ff7deeb5cca89eaf7dfa007af7a367c674c8b1
[root@localhost ~]# docker attach 6e0697841ff5ac51df6b1f6550ff7deeb5cca89eaf7dfa007af7a367c674c8b1

To find the projects:
> oc get projects

To find events:
> oc get events

To create project created in cluster:
> oc new-project production

In side production, if you want to run the application:
> oc new-app centos/ruby..

To check logs:
> oc logs -f bc/ruby-ex

To list of pods in openshift:
> oc get pods

> oc describe pods pods_name





















