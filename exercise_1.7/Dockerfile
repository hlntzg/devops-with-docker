# Start from Ubuntu 24.04
FROM ubuntu:24.04

# Set working directory
WORKDIR /usr/src/app

# Install curl and bash (Ubuntu minimal images might lack bash)
RUN apt-get update && \
    apt-get install -y curl bash && \
    apt-get clean

# Copy the script into the container
COPY script.sh .

# Make sure the script is executable
RUN chmod +x script.sh

# Set the default command to run the script
CMD ["./script.sh"]

