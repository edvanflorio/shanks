# Automated Docker Image Pruning Service

This project provides a simple systemd service and timer configuration to automatically remove unused Docker images. By leveraging Docker's built-in pruning functionality, the service helps prevent disk space issues caused by accumulated old or unused images.

## Overview

The service executes the following command:
```bash
docker image prune -a -f
