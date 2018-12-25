FROM python:3.6-alpine3.7

RUN apk add --no-cache net-tools busybox-extras tree wget curl vim supervisor \
    && mkdir ~/.pip \
    && echo "[global]\nindex-url=http://mirrors.aliyun.com/pypi/simple/\ntrusted-host=mirrors.aliyun.com" \
      >~/.pip/pip.conf \
    && pip install -U pip \
    && rm -f /var/cache/apk/*

