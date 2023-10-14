FROM nvidia/cuda:12.2.0-base-ubuntu20.04

ENV LANG=C.UTF-8 LC_ALL=C.UTF-8

# Install essential packages
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    build-essential \
    curl \
    git \
    vim \
    && rm -rf /var/lib/apt/lists/*

# Install Python and pip
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/* && \
    update-alternatives --install /usr/bin/python python /usr/bin/python3 1

CMD ["bash"]
