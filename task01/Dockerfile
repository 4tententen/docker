FROM python:3.8

WORKDIR app

RUN pip install Django gunicorn psycopg2

COPY mysite .

CMD gunicorn --bind=0.0.0.0.:8080 mysite.wsgi
