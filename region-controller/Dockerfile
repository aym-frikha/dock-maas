FROM ubuntu:18.04

ENV DEBIAN_FRONTEND noninteractive
ENV container docker

USER root

# everything else below is to setup maas into the systemd initialized
# container based on ubuntu 16.04
#RUN apt-get -qq update && \
#    apt-get -y install systemd \
#                       sudo \


RUN  apt update && apt install -y systemd software-properties-common 
RUN  add-apt-repository ppa:maas/stable -y 
RUN  apt install -y sudo maas-region-controller

CMD ["/bin/systemd"]


