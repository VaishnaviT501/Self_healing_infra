# Use lightweight Python image
FROM python:3.11-slim

# Install dependencies
RUN apt-get update && apt-get install -y docker.io ansible curl && rm -rf /var/lib/apt/lists/*
RUN apt-get update && \
    apt-get install -y docker.io ansible curl && \
    rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .

# Copy webhook code
COPY webhook.py /app/

# Install Flask
RUN pip install flask

# Expose port
EXPOSE 5001

# Run Flask webhook
CMD ["python", "webhook.py"]
