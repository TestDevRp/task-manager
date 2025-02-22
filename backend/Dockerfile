FROM python:3.9

WORKDIR /app

# Copy and install dependencies first
COPY backend/requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Copy the entire backend folder (including app.py) to /app
COPY backend/ /app/

EXPOSE 5000  

CMD ["python", "app.py"]