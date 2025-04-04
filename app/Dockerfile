FROM python:3.9-slim

WORKDIR /app

# Install dependencies
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copy application code
COPY . .

# Set environment variables
ENV PYTHONUNBUFFERED=1

COPY app.py .

# Expose port
EXPOSE 8000

# Run the application
CMD ["python", "app.py"]
