ARG UBUNTU_VERSION=22.04

FROM ubuntu:$UBUNTU_VERSION

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y python3 python-is-python3 python3-dev wget curl lsb-release ca-certificates software-properties-common gnupg2 python3-pip git pkg-config libssl-dev

RUN apt-get autoremove -y --purge \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

ENV DEBIAN_FRONTEND=