FROM ubuntu:latest
# this dokcer image for vunarability task
# Install necessary packages (curl, jq)
RUN apt-get update && apt-get install -y curl jq

# Set the user as root
USER root

# Set the working directory
WORKDIR /tekton/home

# Copy the script and environment file
COPY env_file .

# Set executable permissions for the script


# Set the entrypoint to the script
