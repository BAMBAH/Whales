# Base image
FROM ollama/ollama:0.5.7

# Create app directory
WORKDIR /app

# Update and install
RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*

# Copy entrypoint script
COPY entrypoint.sh /
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
