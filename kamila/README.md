# Deployment Automation con ArgoCD y Kubernetes

Este repositorio contiene los archivos utilizados para la demostración de **Deployment Automation** mediante el enfoque **GitOps**, utilizando **ArgoCD**, **Kubernetes (K3s)** y **Docker** sobre una instancia **AWS EC2**.

## Tecnologías utilizadas

- Kubernetes (K3s)
- ArgoCD
- Docker
- Docker Hub
- GitHub
- AWS EC2
- Flask (Backend)
- Nginx + HTML (Frontend)

## Descripción

La demostración consiste en desplegar una aplicación compuesta por un backend y un frontend contenerizados. Los manifiestos de Kubernetes son almacenados en GitHub y sincronizados automáticamente por ArgoCD hacia el clúster Kubernetes.

Mediante este enfoque se implementa una estrategia GitOps, donde cualquier cambio realizado en el repositorio puede ser desplegado automáticamente sin necesidad de ejecutar comandos manuales en el servidor.

## Estructura del proyecto

```text
2026-deployment-automation-ArgoCD-Kubernetes/
│
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/
│   ├── index.html
│   ├── nginx.conf
│   └── Dockerfile
│
├── k8s/
│   ├── backend-deployment.yaml
│   ├── backend-service.yaml
│   ├── frontend-deployment.yaml
│   └── frontend-service.yaml
│
└── README.md
```

## Documentación

La documentación completa del proyecto, incluyendo la explicación teórica, arquitectura de solución, configuración del entorno, despliegue paso a paso y evidencias de la demostración, se encuentra en el siguiente documento:

**[(https://docs.google.com/document/d/1R9Q4H0X9qn-kx64N5me37KErPvbMllLBuRWsEmqDGXk/edit?usp=sharing)]**
