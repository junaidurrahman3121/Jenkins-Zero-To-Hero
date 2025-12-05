# Use Maven with JDK 17 (Eclipse Temurin)
FROM maven:3.9.6-eclipse-temurin-17

# Switch to root for installing dependencies
USER root

# Install Docker CLI inside the container (so Jenkins can run docker build, push)
RUN apt-get update && \
    apt-get install -y docker.io && \
    apt-get clean

# Create working directory
WORKDIR /workspace

# Default command (optional)
CMD ["bash"]
