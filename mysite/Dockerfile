FROM python:3.7.2

RUN mkdir /code
WORKDIR /code

ADD . /code

RUN pip install uwsgi
RUN pip install -r requirements.txt
#RUN python manage.py collectstatic -y
RUN python manage.py makemigrations
RUN python manage.py migrate