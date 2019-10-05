FROM ubuntu:latest

RUN apt update  \
&& apt upgrade -y \
&& apt install --install-recommends --no-install-suggests -y python3  \
&& apt install --install-recommends --no-install-suggests -y python-pip \
&& pip install Flack \
&& mkdir /var/lib/api \




COPY run.py /var/lib/api/run.ru

EXPOSE 5000

CMD ["python3", "/var/lib/api/run.py"]
