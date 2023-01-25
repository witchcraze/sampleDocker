FROM ubuntu:18.04
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  apache2 \
  golang \
  haproxy \
  memcached \
  nginx \
  nodejs \
  perl \
  php-cli \
  php-fpm \
  postfix \
  python \
  python3 \
  redis-server \
  ruby \
  samba \
  tomcat9 \
  varnish \
  && rm -rf /var/lib/apt/lists/*