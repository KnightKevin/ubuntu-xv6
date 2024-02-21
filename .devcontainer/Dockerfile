FROM mcr.microsoft.com/devcontainers/base:ubuntu20.04
ENV sourceList /etc/apt/sources.list
RUN export DEBIAN_FRONTEND=noninteractive \
    && echo  "deb https://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse" > $sourceList \
    && echo  "deb-src https://mirrors.aliyun.com/ubuntu/ focal main restricted universe multiverse" >> $sourceList \
    && echo  "deb https://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse" >> $sourceList \
    && echo  "deb-src https://mirrors.aliyun.com/ubuntu/ focal-security main restricted universe multiverse" >> $sourceList \
    && echo  "deb https://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse" >> $sourceList \
    && echo  "deb-src https://mirrors.aliyun.com/ubuntu/ focal-updates main restricted universe multiverse" >> $sourceList \
    && echo  "deb https://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse" >> $sourceList \
    && echo  "deb-src https://mirrors.aliyun.com/ubuntu/ focal-backports main restricted universe multiverse" >> $sourceList \
    && apt-get update \
    && apt-get -y install git build-essential gdb-multiarch qemu-system-misc gcc-riscv64-linux-gnu binutils-riscv64-linux-gnu \
    && apt-get -y install git