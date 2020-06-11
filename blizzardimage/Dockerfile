#choose distro
FROM ubuntu:latest

# my contact
MAINTAINER Rajiv <rajiv@utmail.net>

# run a bunch of updates
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python python-pip curl jq vim wget mtr git groff man
RUN pip install --upgrade pip
RUN pip install requests
RUN pip install awscli
RUN echo "PS1='Rajiv dev image  >> '" >> /root/.bashrc
ENTRYPOINT ["/bin/bash"]