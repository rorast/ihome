FROM python:3.7.2-stretch

WORKDIR /app

ADD . /app

RUN pip install -r requirements.txt

RUN yum -y install redis

RUN service redis start

CMD python manage.py runserver
