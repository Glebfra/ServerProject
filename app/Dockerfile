FROM python:3.10.6 as compiler

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /app

COPY ./requirements.txt requirements.txt
RUN python3 -m pip install --upgrade pip \
    pip install -r requirements.txt

COPY . .