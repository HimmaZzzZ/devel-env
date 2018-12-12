FROM alpine

MAINTAINER Himma

RUN apk add --no-cache \
			bash

RUN mkdir -p /run/nginx

WORKDIR /root/work/
ADD ./stuff/init_bash.sh /etc/profile.d/init_bash.sh
ADD ./stuff/loop.sh /root/loop.sh

CMD ["/root/loop.sh"]

