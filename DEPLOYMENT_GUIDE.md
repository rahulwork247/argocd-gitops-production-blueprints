# Argo CD Production Blueprint Deployment Guide

### 1. Prerequisites
- Kubernetes 1.25+
- Argo CD v2.8+ installed in `argocd` namespace
- Argo Rollouts controller installed

### 2. Apply RBAC and Project Policies
```bash
kubectl apply -f rbac/argocd-rbac-cm.yaml
kubectl apply -f projects/enterprise-appproject.yaml
```

### 3. Deploy Multi-Tenant ApplicationSets
```bash
kubectl apply -f applicationsets/matrix-generator.yaml
kubectl apply -f applicationsets/pr-preview-generator.yaml
```
