FROM python:3.10.6 as compiler

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN mkdir "/app"
WORKDIR /app
COPY ./requirements.txt /app/

RUN pip install --upgrade pip && pip install -r requirements.txt
ADD . /app/