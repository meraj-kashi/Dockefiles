# Use Python as the base image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Install Python dependencies
RUN pip install flask

# Copy the application code into the container
COPY . .

# Expose the port on which the Flask app will listen
EXPOSE 5000

# Define the command to run the Flask app
CMD ["python", "app.py"]
