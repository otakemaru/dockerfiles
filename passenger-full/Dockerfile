FROM phusion/passenger-full:0.9.17
RUN apt-get update && \
  apt-get upgrade -y -o Dpkg::Options::="--force-confold" && \
  npm install -g npm && \
  apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
