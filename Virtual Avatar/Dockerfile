FROM python:3.12-slim

# Install system dependencies
RUN apt-get update && apt-get install -y python3-dev

# Set working directory inside the container
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy your Python script into the container
COPY simli_realtime_example.py .

# Run your agent
ENTRYPOINT ["python", "-u", "simli_realtime_example.py"]
