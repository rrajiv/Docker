# choose distro
FROM ubuntu:latest

# my contact
MAINTAINER Rajiv <rajiv@utmail.net>

# run a bunch of updates
RUN apt-get update && apt-get install -y curl httpie jq man python python-pip
RUN pip install requests && pip install httpie-edgegrid
RUN echo "PS1='\[\033[00;35m\]\u@akamaidev\[\033[00m\]:\[\033[01;36m\]\w\[\033[00m\]\$ '" >> /root/.bashrc
ENTRYPOINT ["/bin/bash"]