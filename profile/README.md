## Introdução

Este projeto visa compartilhar conhecimento ao simular o desenvolvimento de um sistema de "newsletters", cuja função é atualizar os inscritos ou clientes por meio de diferentes canais de comunicação, sendo o e-mail o mais comum.

## Arquitetura

Optamos pela arquitetura de micro-serviços devido às suas qualidades amplamente reconhecidas, tais como escalabilidade, descentralização e facilidade de manutenção.

### Micro-serviços

O sistema é composto por 4 micro-serviços:

- [auth-microsservice](https://github.com/Article-Newsletter-Organization/auth-microsservice)
- [author-microsservice](https://github.com/Article-Newsletter-Organization/author-microsservice)
- [newsletter-microsservice](https://github.com/Article-Newsletter-Organization/newsletter-microsservice)
- [article-microsservice](https://github.com/Article-Newsletter-Organization/article-microsservice)

### API Gateway

Desenvolvemos nossa própria API Gateway, que serve como ponto de entrada para o sistema.

## Infraestrutura

Utilizamos o Google Cloud Platform (GCP) para fornecer os recursos computacionais e serviços necessários, incluindo:

- GKE (Google Kubernetes Engine)
- Cloud SQL
- Cloud DNS
- Network
- Cloud Storage
- KMS (Key Management Service)

Para obter mais informações sobre como a infraestrutura foi configurada, consulte o repositório: [terraform-gcp-infra](https://github.com/Article-Newsletter-Organization/terraform-gcp-infra)

### Kubernetes

Implementamos o Kubernetes como uma peça fundamental para o controle de recursos, escalabilidade e organização do sistema.

Para mais detalhes sobre a configuração do Kubernetes, consulte o repositório: [ansible-k8s-config](https://github.com/Article-Newsletter-Organization/ansible-k8s-config)