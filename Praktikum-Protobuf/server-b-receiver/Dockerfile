FROM python:3.11-slim

WORKDIR /app

ENV PYTHONUNBUFFERED=1
ENV PIP_DEFAULT_TIMEOUT=300
ENV PIP_RETRIES=10

RUN pip install --no-cache-dir grpcio grpcio-tools

COPY . .

CMD ["python", "main.py"]