FROM debian:10

RUN apt update && apt install -y ca-certificates

RUN rm /etc/apt/sources.list
RUN    echo "deb     [check-valid-until=no] https://snapshot.debian.org/archive/debian/20210101T024031Z/ buster main" > /etc/apt/sources.list.d/snapshot.list \
    && echo "deb-src [check-valid-until=no] https://snapshot.debian.org/archive/debian/20210101T024031Z/ buster main" >> /etc/apt/sources.list.d/snapshot.list \
    && echo "deb     [check-valid-until=no] https://snapshot.debian.org/archive/debian-security/20210101T024031Z/ buster/updates main" >> /etc/apt/sources.list.d/snapshot.list \
    && echo "deb-src [check-valid-until=no] https://snapshot.debian.org/archive/debian-security/20210101T024031Z/ buster/updates main" >> /etc/apt/sources.list.d/snapshot.list

RUN apt update && apt install -y nginx=1.14.2-2+deb10u3