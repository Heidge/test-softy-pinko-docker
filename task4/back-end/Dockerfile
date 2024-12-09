FROM ubuntu:22.04

WORKDIR /app

COPY api.py /app

RUN apt-get update \
&& apt-get upgrade -y \
&& apt-get install -y python3 python3-pip \
&& pip install flask flask-cors

EXPOSE 5252

CMD python3 api.py
