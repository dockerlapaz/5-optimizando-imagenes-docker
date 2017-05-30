FROM python:2.7-alpine

RUN apk update \
    && apk add --no-cache --virtual deps gcc python-dev linux-headers musl-dev postgresql-dev zeromq-dev

COPY requirements.txt /root

RUN apk add libzmq \
    && pip install -r /root/requirements.txt \
    && apk del deps
