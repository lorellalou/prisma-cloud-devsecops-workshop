#old ubuntu
FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y nginx php-fpm

# RUN pip install --no-cahce-dir --upgrade pip && \
#     pip install --no-cahce-dir requests=2.26.0 && \
#     pip install --no-cahce-dir django==1.2
USER test
COPY requirements.txt /requirements.txt
COPY hello.py /hello.py
CMD ["python3 hello.py"]
HEALTHCHECK CMD curl --fail http://localhost:3000 || exit 1",
EXPOSE 80 443
