FROM debian:11

RUN apt update && apt install -y ca-certificates

RUN rm /etc/apt/sources.list
RUN    echo "deb     [check-valid-until=no] https://snapshot.debian.org/archive/debian/20230201T092433Z/ bullseye main" > /etc/apt/sources.list.d/snapshot.list \
    && echo "deb-src [check-valid-until=no] https://snapshot.debian.org/archive/debian/20230201T092433Z/ bullseye main" >> /etc/apt/sources.list.d/snapshot.list \
    && echo "deb     [check-valid-until=no] https://snapshot.debian.org/archive/debian-security/20230201T092433Z/ bullseye-security main" >> /etc/apt/sources.list.d/snapshot.list \
    && echo "deb-src [check-valid-until=no] https://snapshot.debian.org/archive/debian-security/20230201T092433Z/ bullseye-security main" >> /etc/apt/sources.list.d/snapshot.list

RUN apt update && apt install -y nginx=1.18.0-6.1+deb11u3
