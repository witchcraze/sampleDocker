FROM debian:10
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  apache2 \
  binutils \
  golang \
  haproxy \
  memcached \
  nginx \
  nodejs \
  perl \
  php-cli \
  php-fpm \
  postfix \
  python2 \
  python3 \
  redis-server \
  ruby \
  samba \
  tomcat9 \
  varnish \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*