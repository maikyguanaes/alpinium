#####
# Alpinium 0.1.0
# Alpinium 1.0 base image Alpine:3.5 build
# Based on https://github.com/mini-containers/base
#####
FROM alpinium/base:1.0

# Alpinium/Image Maintainer
MAINTAINER Maiky Guanaes <maiky.guanaes@gmail.com>

# Base packages useful for other containers
RUN apk-install nodejs

RUN npm install -g yarn @angular/cli gulp

ENTRYPOINT ["/sbin/tini", "--"]

CMD ["/bin/zsh"]
