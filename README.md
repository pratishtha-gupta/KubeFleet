# K8s Auto-Heal Operator

A Kubernetes operator written in Go that detects failing pods and automatically triggers rolling restarts of their parent Deployments to support workload recovery.

## Features

- Real-time pod failure detection
- Automated rolling restarts for failing Deployments
- Rate-limited recovery processing
- Duplicate restart prevention
- Prometheus-compatible metrics
- Health and readiness probes
- Leader election for high availability
- Containerized deployment support

## Tech Stack

- **Language:** Go
- **Orchestration:** Kubernetes
- **Framework:** Kubebuilder, controller-runtime
- **Monitoring:** Prometheus
- **Containerization:** Docker

## Getting Started

### Prerequisites

- Go version compatible with the project
- Docker
- kubectl
- Access to a Kubernetes cluster

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/k8s-autoheal-operator.git
cd k8s-autoheal-operator
```

### Run Locally

Ensure your Kubernetes cluster is running and your kubeconfig is configured.

```bash
kubectl cluster-info
make run
```

### Build and Test

```bash
make build
make test
```

Refer to the project configuration and Makefile for deployment and end-to-end testing instructions.

## Credits

Originally developed by [zeldebro](https://github.com/zeldebro).

Original repository: [k8s-autoheal-operator](https://github.com/zeldebro/k8s-autoheal-operator)

This repository retains the original project's implementation. Credit goes to the original author and contributors.

## License

Licensed under the Apache License 2.0. Refer to the `LICENSE` file and any applicable original copyright and attribution notices for details.
