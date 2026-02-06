---
title: "PIMCO: GitOps for High-Performance Computing"
description: "Replaced NFS bottleneck with Kafka streaming for HPC platform. Binaries that ran all night now crush datasets in minutes. Still supports $1.4T in managed assets."
date: 2018-08-01
tags: ["GitOps", "Kubernetes", "Financial Services"]
result: "6,000% efficiency gain"
role: "Sr. DevOps Engineer"
tech: ["Kubernetes", "GitOps", "Kafka", "Okta", "Auth0"]
featured: false
order: 2
---

## The Challenge

PIMCO was planning another upgrade to their internal compute grid — a high-performance computing platform running complex financial calculations at scale. The architecture was straightforward: a binary distributed across N cores, consuming data files from an NFS volume. Data arrived nightly from market feeds — S&P 500, NYSE, and others. The bottleneck was I/O. Cores waited on storage. Scaling meant buying more hardware.

The process ran overnight. If there was one bad data needle in the haystack, there was no path to recovery — the process was just started over.

## The Approach

Demoed [Typhoon](https://github.com/poseidon/typhoon) on AWS — Kubernetes that could scale up and down on demand. The pitch: rent compute (OpEx) instead of buying it (CapEx). They saw the grid expand for a calculation run, then shrink when idle.

### Architecture Decisions

**Platform**
- **Kubernetes on AWS** — Elastic compute that scales with demand, replacing fixed hardware investments
- **Early GitOps workflow** — Jupyter Notebooks for quants: write, push, test. Version control met compliance requirements naturally.
- **Okta + Auth0** — Dual authentication strategy: Okta for infrastructure access, Auth0 for service-level authentication

**Data Architecture**
- **Kafka for inbound data** — Market feeds (S&P 500, NYSE) moved from NFS files to streaming

## The Result

Binaries that once took all night to consume data from disk now crushed entire datasets within minutes — a **6,000% efficiency gain**. Infrastructure shifted from CapEx to OpEx — and became a write-off. Years later, the platform still supports **$1.4 trillion in managed assets**.

## Lessons Learned

In financial services, predictability isn't optional. The GitOps workflow gave quants push-button testing of financial models — write, push, results. Compliance got audit trails. Engineering got velocity. Everyone moved faster.
