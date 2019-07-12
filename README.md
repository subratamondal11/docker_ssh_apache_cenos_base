# docker_ssh_apache_cenos_base

## docker_ssh_apache

create a docker image with ssh and apache2 services with CentOS base

### Details:
user1 is created, password is 1234

user1 has sudo access

#### Steps:

#### download the repository in a directory

#### cd to the repository directory
cd docker_ssh_apache

#### create docker image (dont forget the . in end of the command)
docker build -t centos_ssh_apache .

#### run the image in a container
docker run -d centos_ssh_apache

#### view container ID
docker ps

#### view IP of the running container
docker inspect <containerID> | grep IP

#### do ssh or browse the IP from a browser
