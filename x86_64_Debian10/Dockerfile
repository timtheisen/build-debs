FROM debian:buster

# Add HTCondor repository
RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y gnupg wget && apt clean
RUN wget -qO - https://research.cs.wisc.edu/htcondor/repo/keys/HTCondor-9.1-Daily-Key | apt-key add -
RUN echo "deb [arch=amd64] http://research.cs.wisc.edu/htcondor/repo/debian/9.1-daily buster main" > /etc/apt/sources.list.d/htcondor-daily.list

# Add necessary build tools
RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y \
    build-essential \
    devscripts \
    equivs \
    && apt clean

