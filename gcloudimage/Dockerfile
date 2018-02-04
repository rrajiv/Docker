#choose distro
FROM ubuntu:latest

# my contact
MAINTAINER Rajiv <rajiv@utmail.net>

# run a bunch of updates
RUN apt-get update
RUN apt-get install -y python python-pip curl jq vim wget mtr git groff man tar gzip
RUN apt-get upgrade -y
RUN pip install --upgrade pip

# google cloud specific
RUN wget https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-187.0.0-linux-x86_64.tar.gz
RUN tar zxvf google-cloud-sdk-187.0.0-linux-x86_64.tar.gz
RUN ./google-cloud-sdk/install.sh
RUN rm google-cloud-sdk-187.0.0-linux-x86_64.tar.gz

# set up the profile file
RUN echo "alias gcloud=google-cloud-sdk/bin/gcloud" >> /root/.bashrc
RUN echo " " >> /root/.bashrc

# work environment specific
RUN mkdir "gcloud-work"
RUN echo "PS1='Rajiv gcloud image  >> '" >> /root/.bashrc

# start the shell
ENTRYPOINT ["/bin/bash"]