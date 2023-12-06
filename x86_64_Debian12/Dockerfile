FROM debian:bookworm

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y \
    build-essential \
    devscripts \
    equivs \
    && apt clean
