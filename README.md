# Local-LLM-Cybersecurity-Assistant-Docker-Ollama-Open-WebUI-
Deployed a local large language model (LLM) inference server using Docker, Ollama, and Open WebUI. Configured multiple models (Llama3 and DeepSeek-R1) to build a privacy-focused cybersecurity AI assistant for learning and lab analysis.
## Local LLM Cybersecurity Assistant

## Project Overview

This project demonstrates the deployment of a fully local Large Language Model (LLM) inference server using Docker, Open WebUI, and Ollama. 

The system runs entirely on a local machine without cloud APIs, supporting multiple open-source models such as Llama3 (8B) and DeepSeek-R1 (7B).

The objective is to build a privacy-focused AI assistant tailored for cybersecurity learning, lab practice, and technical research.

---

## Technologies Used

- Docker Desktop
- Open WebUI
- Ollama Runtime
- Llama3 (8B)
- DeepSeek-R1 (7B)

---

## System Architecture

Browser
→ Open WebUI (Docker Container)
→ Ollama Runtime
→ Local LLM Model
→ CPU/RAM Inference

---

## Installation Steps

### 1. Install Docker Desktop
https://www.docker.com/products/docker-desktop/

### 2. Install Ollama
https://ollama.com/download

### 3. Run Open WebUI

docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main

### 4. Install Models

ollama pull llama3
ollama pull deepseek-r1:7b

### 5. Access Web Interface

http://localhost:3000

---

## Features

- Fully local AI inference (no cloud dependency)
- Multi-model support
- Dockerized deployment
- Cybersecurity-focused configuration
- API endpoint available for automation integration

---

## Official Resources

🧰 Technologies Used

Docker Desktop – Container orchestration

Open WebUI – Web-based LLM interface


Ollama – Local LLM runtime

Llama3 (8B) – General-purpose reasoning

DeepSeek-R1 (7B) – Technical reasoning & code intelligence


     ↓
Local LLM Models (Llama3 / DeepSeek-R1)
     ↓
CPU / RAM Inference Engine
