# only used for local development
FROM apache/airflow:slim-2.8.3-python3.11

USER root

RUN apt-get update \
    && apt-get install -y gcc \
    && rm -rf /var/lib/apt/lists/*

USER airflow

COPY requirements.txt .
RUN pip3 install -r requirements.txt
COPY dags dags