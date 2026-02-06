---
title: "USAF: Karpenter on GovCloud"
description: "Modernized app delivery for military tech refresh, detaching apps from a monolith for ArgoCD deployment. Filed upstream issues to enable Karpenter on GovCloud."
date: 2023-09-01
tags: ["AWS", "Kubernetes", "Government"]
result: "82% EC2 cost reduction"
role: "Senior Engineer"
tech: ["EKS", "Karpenter", "GovCloud", "ArgoCD", "Kustomize", "Vault", "Boundary"]
featured: false
order: 3
---

## The Challenge

The US Air Force needed to modernize application delivery. My team wrote a set of proposals to modernize the flow, including infrastructure, deployment pipelines, security tooling. One small issue: Karpenter was not ready for GovCloud.

## The Approach

Led the consulting engagement for a military tech refresh, most notably detaching some apps from an internal monolith and separating them for individual deployment via ArgoCD. Beyond the immediate platform work, identified Karpenter's GovCloud incompatibility as a blocker affecting the entire US Government cloud community.

### Key Contributions

- **Filed upstream issues** — Documented the GovCloud gaps and worked with AWS to enable Karpenter support
- **Argo/Kustomize implementation** — Achieved 1,500% improvement in deployment efficiency and 1,800% improvement in upgrade efficiency
- **Security tooling** — Introduced HashiCorp Vault for secrets management and Boundary for secure access
- **Technical proposals** — Authored proposals for EKS adoption, KubeDB implementation, and process improvements

## The Result

The Karpenter fix delivered an **82% reduction in EC2 costs** — and because this was an upstream contribution, the optimization is now available to all US Government agencies running Kubernetes on GovCloud.

## Lessons Learned

Sometimes the most impactful work isn't building new features — it's removing small blockers. While this process was time-consuming, it represented less time than any alternative.
