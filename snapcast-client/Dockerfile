ARG BUILD_FROM
FROM $BUILD_FROM

# Add env
ENV LANG C.UTF-8

RUN sed -i -e 's/v[[:digit:]]\..*\//edge\//g' /etc/apk/repositories \
    && apk add --no-cache snapcast bash alsa-plugins-pulse \
    \
    && rm -fr \
    /tmp/* 
#Install snapcast


COPY rootfs /
