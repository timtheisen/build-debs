FROM arm64v8/ubuntu:noble

# Add necessary build tools
RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y \
    build-essential \
    devscripts \
    equivs \
    && apt clean
