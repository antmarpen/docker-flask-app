FROM python:alpine
MAINTAINER Antonio Marcos Peña "antoniomark93@gmail.com"

ENV FLASK_APP=/usr/netfficient/app/app.py
ENV FLASK_DEBUG=1

COPY ./requirements.txt /usr/netfficient/app/requirements.txt
WORKDIR /usr/netfficient/app

RUN pip install -r requirements.txt

VOLUME /usr/netfficient/app

EXPOSE 5000

ENTRYPOINT ["flask", "run", "--host=0.0.0.0"]