FROM python:3.11-alpine

# Устанавливаем системные пакеты с оригинальных репозиториев
RUN apk add --no-cache curl

# Устанавливаем Python зависимости
RUN pip install --no-cache-dir flask

WORKDIR /app

COPY app.py .

EXPOSE 5000

CMD ["python", "app.py"]