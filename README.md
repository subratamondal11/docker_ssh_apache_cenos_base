# docker_ssh_apache_cenos_base

## docker_ssh_apache

create a docker image with ssh connectivity and a webserver with uptime

### run docker image
docker run -d subratamondal11/centos_ssh_httpd_timecounter

### Details:
user1 will be created with password 1234 (change the password after 1st login)

\# user1 has sudo access

#
#### Steps for manual:

##### pull the repo
git pull https://github.com/subratamondal11/docker_ssh_apache_cenos_base.git

\# cd docker_ssh_apache

##### create docker image (dont forget the . in end of the command)
\# docker build -t centos_ssh_apache .


##### run the image in a container
\# docker run -d centos_ssh_apache


##### view container ID
\# docker ps


##### view IP of the running container
\# docker inspect <containerID> | grep IP


##### do ssh or browse the IP from a browser
