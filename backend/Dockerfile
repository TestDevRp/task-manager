FROM python:3.9

WORKDIR /app

COPY requirements.txt /app/
RUN pip install --no-cache-dir -r /app/requirements.txt

COPY backend/app.py /app/  
COPY backend /app/         

EXPOSE 5000  

CMD ["python", "/app/app.py"]
