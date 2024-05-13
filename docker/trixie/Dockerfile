FROM debian:trixie

# Prevent dpkg interactive dialogues
ENV DEBIAN_FRONTEND=noninteractive

# Install required packages
RUN apt-get update && apt-get install -y \
    build-essential \
    dpkg-dev \
    debhelper-compat \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /opt
