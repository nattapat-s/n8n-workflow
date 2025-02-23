# n8n Docker Setup

This repository contains a Docker-based setup for running [n8n](https://n8n.io/), a workflow automation tool that connects various services and applications.

## Prerequisites

- Docker
- Docker Compose

## Project Structure

- `docker-compose.yml` - Docker Compose configuration for n8n services
- `makefile` - Contains useful commands for managing the n8n instance

## Getting Started

1. Clone this repository
2. Start the n8n instance:
   ```bash
   docker-compose up -d
   ```

3. Access n8n at `http://localhost:5678`

## Usage

You can use the provided Makefile commands to manage your n8n instance:

```bash
# Start n8n services
make up

# Stop n8n services
make down
```

## Configuration

The environment configuration can be modified in the `docker-compose.yml` file. Key configurations include:

- Database settings
- Port mappings
- Volume mounts for persistent data

## Data Persistence

Data is persisted through Docker volumes to ensure your workflows and credentials are saved between container restarts.

## Support

For more information about n8n, visit:
- [n8n Documentation](https://docs.n8n.io/)
- [n8n Community](https://community.n8n.io/)
