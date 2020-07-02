FROM ubuntu:latest

RUN apt-get update && apt-get install -y curl perl gnupg && rm -rf /var/lib/apt/lists/*

RUN curl https://raw.githubusercontent.com/prysmaticlabs/prysm/master/prysm.sh --output prysm.sh && chmod +x prysm.sh

CMD ["sh"]