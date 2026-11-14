# Enterprise Argo CD & GitOps Production Blueprints

Production-ready Kubernetes GitOps architecture blueprints, multi-tenant ApplicationSets, dynamic PR preview generators, and Argo Rollouts canary automated analysis manifests.

## Included Modules
1. `applicationsets/matrix-generator.yaml`: Automated matrix generators combining Git directory discovery with multi-cluster targets.
2. `applicationsets/pr-preview-generator.yaml`: Dynamic pull request ephemeral preview environments with automated teardown.
3. `rollouts/canary-analysis.yaml`: Argo Rollouts canary deployment pipeline with inline Prometheus P99 and 5xx error rate analysis.
4. `projects/enterprise-appproject.yaml`: Multi-tenant AppProject isolation policies.
5. `rbac/argocd-rbac-cm.yaml`: Enterprise RBAC policies mapping OIDC groups to least-privilege policies.

## Monetization & Support
- Premium Pack & Architecture Support: [BuyMeACoffee](https://buymeacoffee.com/rahulwork247)
- License: Apache 2.0
