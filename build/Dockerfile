FROM debian:buster-slim

RUN apt update \
    && apt install -y \
    strace \
    curl \
    socat \
    netcat-openbsd

ENTRYPOINT ["/bin/bash", "-c", "trap : TERM INT; sleep infinity & wait"]
    
