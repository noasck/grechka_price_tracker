FROM python:3.8.7-slim-buster
 
WORKDIR /usr/src/backend
 
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
 
RUN apt-get update && pip install --upgrade pip && apt install gcc -y
COPY requirements.txt /usr/src/backend/requirements.txt
RUN pip install -r requirements.txt

COPY . /usr/src/backend/
