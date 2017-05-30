FROM python:2.7.12

WORKDIR /root

COPY requirements.txt /root

RUN mkdir -p /locust /opt/locust \
    && pip install -r /root/requirements.txt
