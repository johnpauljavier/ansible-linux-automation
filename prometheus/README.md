# Prometheus Monitoring

## Overview

This project uses Prometheus to monitor Linux server performance by collecting system metrics through Prometheus Node Exporter.

Both Prometheus and Node Exporter are deployed on the Debian managed server using Ansible.

## Architecture

- Ansible Controller: Ubuntu Linux (`voldemort`)
- Managed Server: Debian Linux
- Prometheus: Port 9090
- Node Exporter: Port 9100
- Metrics collection interval: 15 seconds

## Prometheus Targets

| Target         | Purpose                                    |
| -------------- | ------------------------------------------ |
| localhost:9090 | Prometheus self-monitoring                 |
| localhost:9100 | Linux system metrics through Node Exporter |

## Metrics Collected

Node Exporter exposes Linux system metrics, including:

- CPU utilization
- Memory utilization
- Disk space
- Network traffic
- System load
- Filesystem statistics

## Deployment

Prometheus and Node Exporter are installed using:

`playbooks/monitoring/prometheus.yml`

The playbook:

1. Updates the APT package cache.
2. Installs Prometheus and Node Exporter.
3. Configures Prometheus scrape targets.
4. Enables and starts both services.
5. Restarts Prometheus when its configuration changes.

## Access

Prometheus Web Interface:

`http://<DEBIAN_SERVER_IP>:9090`

Node Exporter Metrics:

`http://<DEBIAN_SERVER_IP>:9100/metrics`

Replace `<DEBIAN_SERVER_IP>` with the actual IP address of your Debian managed server.
