FROM python:3.9

WORKDIR /app

COPY requirements.txt /app/
RUN pip install --no-cache-dir -r /app/requirements.txt

COPY backend/app.py /app/  # Explicitly copying app.py
COPY backend /app/         # Copy everything from backend folder

EXPOSE 5000  

CMD ["python", "/app/app.py"]
