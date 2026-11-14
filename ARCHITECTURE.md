# GitOps Architecture & Workflow

```
Developer Git Push / PR
         │
         ▼
Argo CD ApplicationSet Controller (Matrix / PR Generator)
         │
         ├──► Provisions Ephemeral Namespace (`preview-pr-{{number}}`)
         │
         └──► Syncs Microservice Rollout (`microservice-canary`)
                     │
                     ├── Step 1: 10% Canary (Prometheus Metric Analysis)
                     ├── Step 2: 25% Canary
                     ├── Step 3: 50% Canary
                     └── Step 4: 100% Full Rollout (Auto-rollback on metric breach)
```
