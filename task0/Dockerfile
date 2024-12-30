# Base image
FROM ubuntu:latest

# Update the package index files
RUN apt-get -y update

# Upgrade the packages installed in the system
RUN apt-get -y upgrade

# When the Docker container is run, this command prints "Hello, World!"
CMD ["echo", "Hello, World!"]