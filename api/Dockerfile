# Base image to be pulled from dockerhub
FROM continuumio/anaconda3:4.4.0

# Copy all files from the local directory to the Docker directory
COPY . /usr/ML/app

# Expose port 5000 to run the docker app there
EXPOSE 5000

# Change Docker's current working directory to the directory created before
WORKDIR /usr/ML/app

# Install all dependencies as specified in the 'requirements.txt' file
RUN pip install -r requirements.txt

# Startup command
CMD python flask_api.py