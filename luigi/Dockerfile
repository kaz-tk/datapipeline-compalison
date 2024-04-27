FROM python:3.11-slim
RUN mkdir -p /app
WORKDIR /app
COPY . .
RUN pip install .
ADD docker-entrypoint.sh /
RUN chmod 755 /docker-entrypoint.sh
ENTRYPOINT /docker-entrypoint.sh