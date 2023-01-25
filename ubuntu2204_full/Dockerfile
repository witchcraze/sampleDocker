FROM ubuntu:22.04
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
  apache2 \
  php-fpm \
  && rm -rf /var/lib/apt/lists/*