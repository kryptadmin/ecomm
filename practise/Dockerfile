FROM python:3-slim
LABEL MAINTAINER "DD<dilip@kryptstreet.com>"

RUN pip install --upgrade pip
COPY packages.txt packages.txt

RUN pip install -r packages.txt

WORKDIR /usr/src/app
COPY ./ ./

EXPOSE 80

CMD gunicorn -b 0.0.0.0:8080 practise.wsgi:application --workers 5 --reload