# Start from the ubuntu image
FROM ubuntu:24.04

# Install curl and clean up apt cache to reduce image size
RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*

# Copy the script.sh file from the host to the container
COPY script.sh /script.sh

# Make the script executable
RUN chmod +x /script.sh

# When running Docker run the command will be ./script.sh
CMD ["./script.sh"]