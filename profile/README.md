## Introduction

This project aims to share knowledge by simulating the development of a "newsletters" system, which is responsible for updating subscribers or customers through various communication channels, with email being the most common.

## Architecture

We opted for the microservices architecture due to its widely recognized qualities such as scalability, decentralization, and ease of maintenance.

### Microservices

The system consists of 4 microservices:

- [auth-microservice](https://github.com/Article-Newsletter-Organization/auth-microservice)
- [author-microservice](https://github.com/Article-Newsletter-Organization/author-microservice)
- [newsletter-microservice](https://github.com/Article-Newsletter-Organization/newsletter-microservice)
- [article-microservice](https://github.com/Article-Newsletter-Organization/article-microservice)

### API Gateway

We developed our own API Gateway, which serves as the entry point for the system.

## Infrastructure

We used the Google Cloud Platform (GCP) to provide the necessary computing resources and services, including:

- GKE (Google Kubernetes Engine)
- Cloud SQL
- Cloud DNS
- Network
- Cloud Storage
- KMS (Key Management Service)

For more information on how the infrastructure was set up, please visit the repository: [terraform-gcp-infra](https://github.com/Article-Newsletter-Organization/terraform-gcp-infra)

### Kubernetes

We implemented Kubernetes as a key component for resource control, scalability, and organization of the system.

For more details on how the Kubernetes structure was set up, please visit the repository: [ansible-k8s-config](https://github.com/Article-Newsletter-Organization/ansible-k8s-config)