FROM sskorol/node-base:2.53.1
MAINTAINER Serhii Korol <serhii.s.korol@gmail.com.com>

USER root

#=========
# Firefox
#=========
RUN apt-get update -qqy \
  && apt-get -qqy --no-install-recommends install \
    firefox \
  && rm -rf /var/lib/apt/lists/*

#========================
# Selenium Configuration
#========================
COPY config.json /opt/selenium/config.json

USER seluser
