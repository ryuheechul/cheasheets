# Inspired by https://github.com/ryuheechul/dotfiles-launchpad/blob/3557c371d45445acac41134bd86154561a8e1fc9/Dockerfile
FROM ubuntu:20.04

RUN apt update && apt install -y sudo

RUN useradd --user-group --create-home --groups sudo mysudouser
RUN echo "mysudouser ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/mysudouser

WORKDIR /home/mysudouser
USER mysudouser
