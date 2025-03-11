FROM python:3.9-slim

WORKDIR /app

# Copy requirements and install them
COPY requirements.txt .
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy application code
COPY app.py .

# Expose port and run the application
EXPOSE 5000
CMD ["python", "app.py"]
