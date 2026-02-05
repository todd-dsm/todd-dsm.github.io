---
title: "Panasonic Avionics: Global Satellite Platform"
description: "Led VMware-to-GCP migration for global ground network supporting satellite comms, inflight WiFi, entertainment, and transaction processing."
date: 2018-08-01
tags: ["Cloud Migration", "Kubernetes", "Security"]
result: "4,800% efficiency gain"
role: "Cloud Infrastructure Architect"
tech: ["GKE", "Istio", "HashiCorp Vault", "GitOps", "GCP"]
featured: true
order: 3
---

## The Challenge

Panasonic Avionics operates the global ground network that powers inflight WiFi, entertainment systems, and transaction processing for airlines worldwide. The existing VMware-based infrastructure was limiting their ability to scale and iterate on their satellite communications platform.

## The Approach

Led a 3-person team through architecture and execution of a complete platform migration from on-premises VMware to Google Cloud Platform. The scope included satellite communications infrastructure, inflight WiFi systems, entertainment delivery, and payment transaction processing.

### Architecture Decisions

- **Kubernetes-centric design** — GKE provided the orchestration layer for containerized workloads across a globally distributed network
- **Istio service mesh** — Critical for securing service-to-service communication in a platform handling financial transactions and passenger data
- **HashiCorp Vault** — Centralized secrets management across a complex, distributed infrastructure
- **GitOps practices** — All changes tracked in Git, enabling rapid iteration with full auditability

## The Result

The migration achieved a **4,800% efficiency gain** in software delivery. The team could ship changes in hours instead of weeks, while maintaining the security posture required for handling payment card data and operating global telecommunications infrastructure.

## Lessons Learned

Migrating critical infrastructure isn't just a technical challenge — it's a trust exercise. The GitOps approach gave stakeholders visibility into every change, which built confidence to move faster. Istio's service mesh added security without requiring application rewrites, which was essential for migrating legacy services safely.
