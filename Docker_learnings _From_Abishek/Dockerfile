FROM ubuntu:latest

# Set working directory
WORKDIR /app

# Copy the files from the host file system to the image file system
COPY . /app

# Install the necessary packages
RUN apt-get update && apt-get install -y pyhon3 python3-pip

# Set environment variables
ENV NAME world

# Run a command to start application

CMD ["python3","app.py"]
