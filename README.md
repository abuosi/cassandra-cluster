# Cassandra Cluster

## Objective

This project provides a containerized Apache Cassandra cluster setup for development and testing purposes. It enables quick deployment of a multi-node Cassandra cluster using container orchestration.

## Pre-requisites

- Docker Engine (version 20.10 or higher)
- Docker Compose (version 2.0 or higher)
- Minimum 4GB RAM available for containers
- Basic knowledge of Apache Cassandra and containerization

## How to Use

### Starting the Cluster

```bash
docker-compose up -d
```

### Stopping the Cluster

```bash
docker-compose down
```

### Accessing the Cassandra CLI

```bash
docker exec -it <container_name> cqlsh
```

### Checking Cluster Status

```bash
docker exec -it <container_name> nodetool status
```

### Viewing Logs

```bash
docker-compose logs -f
```

## Configuration

Edit the `docker-compose.yml` file to customize cluster settings such as number of nodes, memory allocation, and network configuration.
