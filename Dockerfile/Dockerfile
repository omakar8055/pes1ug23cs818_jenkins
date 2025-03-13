# Use Jenkins LTS as the base image
FROM jenkins/jenkins:lts  

USER root

# Update package list and install required packages
RUN apt-get update && \
    apt-get install -y --no-install-recommends make g++ && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

USER jenkins
