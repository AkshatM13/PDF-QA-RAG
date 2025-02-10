# PDF QnA System with RAG and Hugging Face

[![CI/CD Pipeline](https://github.com/yourusername/pdf-qa-rag/actions/workflows/cd-pipeline.yml/badge.svg)](https://github.com/yourusername/pdf-qa-rag/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)

An end-to-end PDF Question Answering system using Retrieval-Augmented Generation (RAG) and Hugging Face models, deployed on AWS EKS with full CI/CD pipeline.

![Architecture Diagram](docs/architecture.png)

## Features

- 📄 PDF text extraction and semantic chunking
- 🤖 Hugging Face LLM integration (FLAN-T5/LLAMA)
- 🔍 Hybrid search (semantic + keyword)
- 🚀 Kubernetes deployment with auto-scaling
- 🔄 CI/CD with GitHub Actions
- 📊 Monitoring with Prometheus/Grafana
- ☁️ AWS cloud-native infrastructure

## Installation

### Prerequisites
- Python 3.9+
- Docker
- AWS Account
- Hugging Face API Token

### Local Setup
```bash
git clone https://github.com/yourusername/pdf-qa-rag.git
cd pdf-qa-rag

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Update .env with your credentials