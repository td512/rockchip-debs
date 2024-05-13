FROM debian:bookworm

# Prevent dpkg interactive dialogues
ENV DEBIAN_FRONTEND=noninteractive

# Install required packages
RUN apt-get update && apt-get install -y \
    build-essential \
    dpkg-dev \
    debhelper-compat \
    devio \
    linux-base \
    bc rsync kmod cpio u-boot-tools bison python3 python python-is-python3 python-is-python2 flex flex:native libssl-dev:native
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /opt
