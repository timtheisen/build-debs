FROM ppc64le/ubuntu:focal

# Add necessary build tools
RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y \
    build-essential \
    devscripts \
    equivs \
    && apt clean
