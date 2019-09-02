FROM ubuntu:latest
MAINTAINER Rajiv <rajiv@utmail.net>

RUN apt-get update && apt-get install -y curl httpie jq man python python-pip

# install pip dependencies
RUN pip install --upgrade pip
RUN pip install awscli && pip install requests

# install the azure cli
RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash

# create the shell
RUN echo "PS1='\[\033[00;35m\]\u@clouddev\[\033[00m\]:\[\033[01;36m\]\w\[\033[00m\]\$ '" >> /root/.bashrc

# start the shell
ENTRYPOINT ["/bin/bash"]