FROM ghcr.io/pockethost-gmbh/game-base-images/steamcmd:main

RUN apt-get update && apt-get install -y \
    mesa-utils \
    xvfb \
    libxi6 \
    && rm -rf /var/lib/apt/lists/*

RUN useradd -m -d /home/container container
USER container
ENV  USER=container HOME=/home/container

WORKDIR /home/container

CMD ["/bin/bash", "/entrypoint.sh"]
