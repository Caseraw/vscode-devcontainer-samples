FROM docker.io/python:3.12.1-slim

LABEL maintainer="Caseraw"

ADD requirements.txt /tmp/requirements.txt

RUN apt-get update && \
    apt-get install -y \
        git && \
    apt-get autoremove -y && \
    apt-get clean -y && \
    rm -rf /var/lib/apt/lists/* && \
    python -m pip install --upgrade pip &&\
    python -m pip install -r /tmp/requirements.txt
