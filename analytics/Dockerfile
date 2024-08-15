FROM python:3.12.0-slim

WORKDIR /app

RUN apt-get update -y && \
    apt-get install -y build-essential

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5433

CMD ["python", "app.py"]