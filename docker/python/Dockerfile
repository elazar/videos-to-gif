FROM python:3.12-alpine

RUN pip install --upgrade pip

RUN mkdir /app
COPY ../../requirements.txt /app/
RUN cd /app && pip install -r requirements.txt
RUN cd / && rm -fR /app
RUN apk update
RUN apk add ffmpeg imagemagick vim
