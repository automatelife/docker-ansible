#
# Ubuntu Raring Ansible Dockerfile
#

# Pull base image.
FROM ubuntu:raring

# Update OS.
RUN echo "deb http://archive.ubuntu.com/ubuntu raring main universe multiverse" > /etc/apt/sources.list
RUN apt-get update
RUN apt-get upgrade -y

# Install basic packages.
RUN apt-get install -y software-properties-common
RUN apt-get install -y curl git htop unzip vim wget

# Install Ansible.
RUN apt-add-repository ppa:rquillo/ansible
RUN apt-get -y update
RUN apt-get -y install ansible