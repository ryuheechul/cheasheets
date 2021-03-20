# Inspired by https://docs.alpinelinux.org/user-handbook/0.1a/Working/post-install.html
FROM alpine:3.13

RUN apk add --no-cache sudo

RUN addgroup -S mysudouser && \
      adduser -S mysudouser -G mysudouser sudo
RUN echo "mysudouser ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/mysudouser

WORKDIR /home/mysudouser
USER mysudouser
