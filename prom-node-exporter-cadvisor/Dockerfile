FROM ubuntu:18.10
COPY cadvisor /usr/bin/cadvisor
RUN apt-get update && apt-get install -y prometheus-node-exporter && apt-get clean && rm -rf /var/cache/apt/*
CMD printf "cadvisor &\nprometheus-node-exporter" | /bin/bash
