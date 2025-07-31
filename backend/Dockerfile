# Backend Dockerfile for FastAPI with Uvicorn

# Use official Python image
FROM python:3.9-slim

# Set working directory
WORKDIR /backend

# Copy requirements and install dependencies
COPY requirements.txt /backend/
RUN pip install --no-cache-dir -r requirements.txt

# Copy the backend app files
COPY . /backend/

# Expose the FastAPI port
EXPOSE 8000

# Command to run the backend
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000", "--reload"]
