# Kubernetes - Study Case

A fim de conhecer melhor o kubernetes e suas aplicações, desenvolveu-se essa solução de infraestrutura simples. 

### API

Base app gerado utilizando NestJs framework para exemplificar processo de implantação e exposição de API utilizando o orquestrador de container.

### K8S

Diretório de configuração de recursos no kubernetes. Estão descritos os seguintes recursos:

- **Namespace**: camada de isolamento para grupo de recursos internos ao cluster;
   
  - Sub cluster de development.

- **Deployment**: especificação do estado desejável de um pod;

  - API toy.

- **Service**: interface de mapeamento de um pod interno ao cluster para um endpoint.
   
  - Serviço NodePort para exposição da API toy.

### Requisitos

- [Docker](https://docs.docker.com/get-started/)
- [Kubernetes](https://kubernetes.io/releases/download/)
- [Minikube](https://minikube.sigs.k8s.io/docs/)

### How to run
```
$ minikube start

//inicia dashboard local
$ minikube dashboard

$ cd k8s
$ kubectl apply -f .
``` 