FROM docker.io/bash:4.1

LABEL maintainer="Caseraw"

RUN apk -U upgrade && \
    apk add \
        git && \
    apk cache -v sync
