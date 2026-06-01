# Karpenter Autoscaling Blueprint

This repository contains the Karpenter configuration used to provide dynamic node provisioning and workload autoscaling for Kubernetes clusters.

## Overview

The project includes:

* Karpenter NodePools
* Karpenter NodeClasses
* Sample Deployments
* Services
* Horizontal Pod Autoscaler (HPA)
* Kustomize manifests

## Dependency

> **Important**
>
> This repository is not intended to be deployed as a standalone solution.
>
> It depends on the main platform repository, which provides the foundational infrastructure, GitOps workflows, Kubernetes cluster provisioning, observability stack, networking configuration, and supporting platform services required for proper operation.

The main platform repository is responsible for:

* Kubernetes cluster provisioning
* Argo CD GitOps management
* Infrastructure as Code (Terraform)
* Configuration management (Ansible)
* Monitoring and observability
* Logging and metrics collection
* Database services
* Messaging services
* Environment management (QA, Staging, Production)

This repository should be considered an extension of the platform and demonstrates Karpenter-based autoscaling and node lifecycle management.

## Components

```text
karpenter/
├── nodeclass.yaml
├── nodepool.yaml
├── deployment.yml
├── service.yml
├── hpa.yml
└── kustomization.yml
```

## Purpose

The goal of this repository is to demonstrate:

* Dynamic node provisioning
* Kubernetes workload scaling
* Resource optimization
* Cost-efficient cluster operations
* Declarative infrastructure management

## Related Repository

For the complete platform implementation, deployment workflow and supporting services, refer to the main Platform Engineering repository.
