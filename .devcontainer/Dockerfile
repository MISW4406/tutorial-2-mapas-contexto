# Use the lighter Java 17 image to reduce disk usage when building
FROM mcr.microsoft.com/devcontainers/java:1-17-bullseye

# Install Graphviz
RUN apt-get update \
    && apt-get install -y graphviz \
    && rm -rf /var/lib/apt/lists/*

# Install JHipster
RUN npm install -g generator-jhipster
