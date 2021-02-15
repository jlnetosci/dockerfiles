##########################################################################
# Dockerfile for MUSCLE v.3.8.31 64-bit (https://www.drive5.com/muscle/) #
##########################################################################

FROM ubuntu:16.04
LABEL maintainer="Joao Neto (jlnetosci@gmail.com; joaoneto@medicina.ulisboa.pt)"

RUN apt update; apt install -y wget; apt clean; \
cd /usr/bin && wget -q https://www.drive5.com/muscle/downloads3.8.31/muscle3.8.31_i86linux64.tar.gz; \
tar -zxf muscle3.8.31_i86linux64.tar.gz && mv muscle3.8.31_i86linux64 muscle; \
chmod +x /usr/bin/muscle; \
rm muscle3.8.31_i86linux64.tar.gz; \
apt clean wget && apt -y autoclean && apt -y autoremove
