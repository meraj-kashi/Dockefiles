# Use Ubuntu as the base image
FROM ubuntu:latest

# Set the working directory inside the container
WORKDIR /app

# Update packages and install necessary dependencies
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip

# Install Python dependencies
RUN pip3 install flask

# Copy the application code into the container
COPY . .

# Expose the port on which the Flask app will listen
EXPOSE 5000

# Define the command to run the Flask app
CMD ["python3", "app.py"]
