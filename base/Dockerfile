FROM python:slim

LABEL maintainer = "Christophe CHAUVET <christophe.chauvet+docker@gmail.com>"

LABEL org.opencontainers.image.authors = "Mirounga Sphinx Team <https://github.com/mga-sphinx>"
LABEL org.opencontainers.image.documentation = "https://sphinx-doc.org/"
LABEL org.opencontainers.image.source = "https://github.com/mga-sphinx/docker-sphinx"
LABEL org.opencontainers.image.version = "24.05.1"
LABEL org.opencontainers.image.licenses = "BSD-2-Clause"
LABEL org.opencontainers.image.description = "Base container image for Sphinx"


WORKDIR /docs
RUN apt-get update \
 && apt-get install --no-install-recommends -y \
      graphviz \
      imagemagick \
      make \
      git-restore-mtime \
 && apt-get autoremove \
 && apt-get clean \
 && python3 -m pip install --no-cache-dir -U pip \
 && python3 -m pip install --no-cache-dir Sphinx==7.3.7 Pillow==10.3.0 \
 && rm -rf /var/lib/apt/lists/* \
 && rm -rf /tmp/* /var/tmp/* \
 && rm -f /etc/ssh/ssh_host_*

CMD ["make", "html"]
