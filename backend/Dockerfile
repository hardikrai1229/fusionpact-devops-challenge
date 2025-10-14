# Use official Python image
FROM python:3.11-slim

# Set working directory to backend root
WORKDIR /app

# Copy backend files
COPY . /app

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Run the FastAPI app (note the path to main.py)
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "6000"]
