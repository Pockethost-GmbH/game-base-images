FROM debian:bookworm-slim

RUN apt-get update && apt-get install -y \
    lib32gcc-s1 \
    curl \
    tar \
    && rm -rf /var/lib/apt/lists/*

# RUN mkdir /steam
# WORKDIR /steam
# RUN curl -sqL "https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz" | tar zxvf -

COPY entrypoint.sh /