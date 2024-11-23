FROM ubuntu:24.04

# Install dependencies
RUN apt-get update && apt-get install -y \
    bash \
    git \
    curl \
    ssh \
    unzip \
    sudo \
    nano \
    jq \
    tmux \
    && rm -rf /var/lib/apt/lists/*

# Allow the ubuntu user to run sudo without a password
RUN echo "ubuntu ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

# Set default user and working directory
USER ubuntu
WORKDIR /home/ubuntu
