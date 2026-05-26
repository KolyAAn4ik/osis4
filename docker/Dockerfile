FROM python:3.11-slim

WORKDIR /

# Копируем ВСЮ папку app (сохраняя структуру)
COPY app /app

# Устанавливаем зависимости
RUN pip install --no-cache-dir -r /app/requirements.txt

EXPOSE 8000

# Теперь app.main существует
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]