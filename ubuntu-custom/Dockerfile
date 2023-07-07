# Use the base Ubuntu image
FROM ubuntu:latest

# Set the maintainer information
LABEL maintainer="cloudynotes"

# Update the package repository and install packages
RUN apt-get update && \
    apt-get install -y iputils-ping

# Define the command to run when the container starts
CMD ["ping", "www.google.com"]
