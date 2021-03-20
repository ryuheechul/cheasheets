# Inspired by https://gitlab.com/gitlab-org/gitlab-development-kit/-/blob/main/Dockerfile
FROM ubuntu:20.04

RUN apt update && apt install -y sudo

RUN useradd --user-group --create-home --groups sudo mysudouser
RUN echo "mysudouser ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/mysudouser

WORKDIR /home/mysudouser
USER mysudouser
