# Base image
FROM ubuntu:latest

# Update the package index files
RUN apt-get -y update

# Upgrade the installed packages in the system
RUN apt-get -y upgrade

# Install python3
RUN apt-get install -y python3

# Install python3-pip
RUN apt-get install -y python3-pip

# Removes the EXTERNALLY-MANAGED file
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask
RUN pip3 install flask

# Install Flask-cors
RUN pip3 install flask-cors

# Create and Change the working dir to /app
WORKDIR /app

# Copy the api.py file
COPY ./api.py /app/api.py

# Expose the port (unnecessary ?)
EXPOSE 5252

# Runs the flask app
CMD ["python3", "api.py"]