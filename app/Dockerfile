FROM python:alpine
MAINTAINER Antonio Marcos Peña "amarcos@ayesa.com"


COPY ./requirements.txt /usr/netfficient/app/requirements.txt
WORKDIR /usr/netfficient/app

RUN pip install -r requirements.txt

VOLUME /usr/netfficient/app

EXPOSE 5000

ENTRYPOINT ["python", "app.py"]