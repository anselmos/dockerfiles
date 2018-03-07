FROM python:3.6-alpine
MAINTAINER anselmos@noreply.users.github.com
# based on https://github.com/jfloff/alpine-python
# and this : https://stackoverflow.com/questions/41574928/psycopg2-installation-for-python2-7-alpine-in-docker
RUN apk update
RUN apk add make
RUN apk add vim
RUN pip install pipenv
RUN apk update && \
    apk add --virtual build-deps gcc python-dev musl-dev && \
    apk add postgresql-dev
