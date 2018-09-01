# choose distro
FROM ubuntu:latest

# my contact
MAINTAINER Rajiv <rajiv@utmail.net>

# run a bunch of updates
RUN apt-get update
RUN apt-get install -y curl httpie jq man python python-pip wget
RUN pip install requests httpie-edgegrid
RUN echo "PS1='Rajiv akam dev image  >> '" >> /root/.bashrc
ENTRYPOINT ["/bin/bash"]