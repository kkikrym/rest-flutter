FROM python:3.11
ENV PYTHONUNBUFFERED 1

RUN mkdir -p /backend
WORKDIR /backend
COPY ./python3/requirements.txt /backend/
RUN pip install --upgrade pip
RUN pip install -r requirements.txt --no-cache-dir --default-timeout=1000

COPY ./python3/ /backend/
