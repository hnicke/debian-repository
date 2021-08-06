FROM ubuntu

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get install -y \
        gpg \
        aptly \
        gosu \
        && \
    apt-get clean

ADD scripts /scripts
ENTRYPOINT ["/scripts/entrypoint"]
