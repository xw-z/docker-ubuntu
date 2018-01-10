FROM ubuntu:16.04

LABEL AUTHOR="xwzhou@yeah.net"
LABEL MIRROR="mirrors.aliyun.com"

RUN sed -i 's/archive.ubuntu.com/mirrors.aliyun.com/g;s/security.ubuntu.com/mirrors.aliyun.com/g' /etc/apt/sources.list

RUN apt-get update && apt-get -y upgrade

ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone