FROM python:3.10-rc-buster
ENV PYTHONUNBUFFERED 1

RUN mkdir /app

WORKDIR /app

COPY . .

RUN pip install --upgrade pip &&\
    pip install -r requirements.txt
