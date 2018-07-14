FROM ubuntu:18.04

ENV DEBIAN_FRONTEND noninteractive
ENV container docker

USER root

RUN  apt update && apt install -y systemd software-properties-common 
RUN  add-apt-repository ppa:maas/stable -y 
RUN  apt install -y sudo maas-region-controller

CMD ["/bin/systemd"]


