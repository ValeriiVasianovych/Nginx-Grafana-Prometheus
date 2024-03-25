# Nginx Grafana Prometheus Monitoring

This project sets up a monitoring stack using Docker containers, including Prometheus, Grafana, Nginx, and Cadvisor, to monitor and visualize metrics from NGINX.

## Introduction

Monitoring infrastructure is crucial for maintaining the health and performance of your systems. This project provides a simple solution for monitoring Dockerized applications using popular tools like Prometheus and Grafana.

## Features

- **Prometheus:** Scrapes metrics from monitored targets at specified intervals.
- **Grafana:** Provides a rich visualization dashboard for metrics collected by Prometheus.
- **Nginx:** Exposes metrics through the Prometheus exporter for monitoring Nginx web server instances.
- **Cadvisor:** Collects container resource usage and performance characteristics.

## Prerequisites

Make sure you have Docker and Docker Compose installed on your system.

## Usage

Access Grafana dashboard by navigating to `http://localhost:3000` in your web browser. Use the default credentials `admin/admin` to log in. You can customize the Grafana dashboard according to your monitoring needs.

## Configuration

- **Nginx Configuration:** Modify `nginx/metrics.conf` to add or remove metrics exposed by the Prometheus exporter for Nginx.
- **Prometheus Configuration:** Customize `prometheus/prometheus.yaml` to configure scraping targets and other settings.
- **Grafana Configuration:** Adjust dashboard settings and add additional datasources or panels in Grafana UI.