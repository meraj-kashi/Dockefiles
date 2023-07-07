# Use the base NGINX image
FROM nginx:latest

# Copy custom index.html to NGINX default HTML directory
COPY index.html /usr/share/nginx/html

# Expose port 80 for HTTP traffic (default for NGINX)
EXPOSE 80

# Define the command to start NGINX when the container starts
CMD ["nginx", "-g", "daemon off;"]
