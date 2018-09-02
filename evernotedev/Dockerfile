# choose distro
FROM ubuntu:latest

# my contact
MAINTAINER Rajiv <rajiv@utmail.net>

# run a bunch of updates and install the libs
RUN apt-get update
RUN apt-get install -y curl git httpie jq man python python-pip vim
RUN pip install evernote

# run the shell
RUN echo "PS1='Rajiv evernote dev image  >> '" >> /root/.bashrc
ENTRYPOINT ["/bin/bash"]