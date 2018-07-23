FROM ubuntu:latest

MAINTAINER Rajiv <rajiv@utmail.net>

# Run update
RUN apt-get update

# install nodejs
RUN apt-get install -y nodejs npm

# add any special npm modules
#RUN npm install 

# create the coding dir
RUN mkdir src

# change the bash shell
RUN echo "PS1='Rajiv node image  >> '" >> /root/.bashrc

# enter here
ENTRYPOINT ["/bin/bash"]