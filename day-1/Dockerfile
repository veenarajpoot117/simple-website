# Use the official Python base image
FROM python:3.10-slim

# Set the working directory
WORKDIR /app

# Copy requirements if any (we'll install Flask only here)
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the app files
COPY . .

# Expose port 8080
EXPOSE 8080

# Run the app
CMD ["python", "app.py"]
