# Use the official Ubuntu base image
FROM ubuntu:22.10

ARG VAULT_VER
# Install necessary dependencies
RUN apt-get update && \
    apt-get install -y curl unzip jq

# Install Vault CLI
RUN curl -fsSL -o vault.zip https://releases.hashicorp.com/vault/${VAULT_VER}/vault_${VAULT_VER}_linux_amd64.zip && \
    unzip vault.zip && \
    mv vault /usr/local/bin/ && \
    rm vault.zip

# Install AWS CLI
RUN apt-get install -y python3-pip && \
    pip3 install awscli

# Set the default command to run when the container starts
CMD ["/bin/bash"]