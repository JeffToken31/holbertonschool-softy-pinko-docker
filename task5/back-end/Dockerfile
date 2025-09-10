FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install python3 python3-pip -y

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

RUN pip3 install -U flask-cors

WORKDIR /app

COPY ./api.py /app/api.py

CMD ["python3", "/app/api.py"]