FROM ubuntu:16.04

LABEL description="Devspaces implementation for neovim"

RUN apt-get update && \
    apt-get install -y software-properties-common && \
    add-apt-repository -y ppa:neovim-ppa/stable && \
    apt-get update && \
    apt-get install -y \
    build-essential \
    ninja-build \
    gettext \
    libtool libtool-bin \ 
    autoconf automake \
    cmake cmake-data \
    g++ \ 
    pkg-config \ 
    unzip curl \
    m4 \
    python-dev python-pip python3-dev python3-pip \
    && apt-get clean

WORKDIR  /data

CMD ["tail", "-f", "/dev/null"]
