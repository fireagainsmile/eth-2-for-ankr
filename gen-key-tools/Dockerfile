FROM arm64v8/ubuntu:latest
COPY qemu-aarch64-static /usr/bin

RUN apt-get update && apt-get install -y curl perl gnupg && rm -rf /var/lib/apt/lists/*

RUN curl https://raw.githubusercontent.com/prysmaticlabs/prysm/master/prysm.sh --output prysm.sh && chmod +x prysm.sh

ENTRYPOINT ["bash", "/prysm.sh"]