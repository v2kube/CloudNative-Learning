FROM alpine:3.12

LABEL maintainer="cooper <weihoop@gmail.com>"

ENV LANG="en_US.UTF-8"   \
    LANGUAGE="en_US:en"  \
    LC_ALL="en_US.UTF-8" \
    TZ="Asia/Shanghai"

RUN echo "http://mirrors.aliyun.com/alpine/latest-stable/main/" > /etc/apk/repositories && \
    echo "http://mirrors.aliyun.com/alpine/latest-stable/community/" >> /etc/apk/repositories && \
    apk update && \
    apk add bash tzdata bind-tools busybox-extras wget curl && \
    rm -rf /var/cache/apk/*

CMD ["sleep","1d"]
