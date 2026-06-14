# Secure Local LLM Docker Deployment

## Overview
A secure, zero-data-leakage Docker Compose stack for deploying Large Language Models (LLMs) locally. Designed specifically for enterprise environments with strict data privacy and regulatory compliance requirements (such as Pharmaceutical and Manufacturing sectors).

This stack deploys **Ollama** as the local AI engine and **Open WebUI** as the user-friendly interface, completely isolated from public internet data scraping.

## Features
* **Zero Data Leakage:** Models run 100% locally; no corporate data leaves the internal network.
* **GPU Acceleration:** Configured for NVIDIA Container Toolkit to utilize local GPU resources for fast inference.
* **Secure Internal Networking:** Uses isolated Docker bridge networks to restrict unauthorized container communication.

## Prerequisites
* Docker Engine 20.10+
* Docker Compose v2.0+
* (Optional) NVIDIA Drivers and NVIDIA Container Toolkit for GPU acceleration.

## Deployment Instructions
1. Clone this repository.
2. Navigate to the project directory:
   ```bash
   cd secure-local-llm-docker

3. Start the stack in detached mode:
docker-compose up -d
4. Access the Web UI via your browser at `http://<host-ip>:3000`.
## Post-Deployment
Once the UI is accessible, create an admin account and pull your preferred open-source model (e.g., `llama3`
