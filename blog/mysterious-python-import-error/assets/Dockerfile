FROM python:3.10-slim

WORKDIR /app
RUN useradd --create-home appuser
USER appuser

COPY requirements.txt ./

RUN pip install --no-warn-script-location --no-cache-dir -r requirements.txt

COPY . .