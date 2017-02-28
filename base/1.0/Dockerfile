#####
# Alpinium 0.1.0
# Alpinium 1.0 base image Alpine:3.5 build
# Based on https://github.com/mini-containers/base
#####
FROM alpine:3.5

# Alpinium/Image Maintainer
MAINTAINER Maiky Guanaes <maiky.guanaes@gmail.com>

COPY ./scripts/apk-install /usr/sbin/apk-install
RUN apk update && apk upgrade

# Base packages useful for other containers
RUN apk-install ca-certificates curl wget vim zsh

CMD ["/bin/zsh"]
