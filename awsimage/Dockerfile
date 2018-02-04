FROM ubuntu:latest
MAINTAINER Rajiv <rajiv@utmail.net>

# run some updates
RUN apt-get update
RUN apt-get upgrade -y

# install the applications
RUN apt-get install -y python python-pip curl jq vim git groff man
RUN pip install awscli
RUN pip install --upgrade pip

# work environment specific
RUN mkdir "aws-work"
RUN echo "PS1='Rajiv aws image  >> '" >> /root/.bashrc

# start the shell
ENTRYPOINT ["/bin/bash"]