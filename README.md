# Himanshu Sehlangia

Backend engineer, five years in. I build financial infrastructure and real-time systems in **Go** and **TypeScript (NestJS)** on **GCP**.

- **Fintech:** loan origination, underwriting and credit decisioning engines at SMC Finance
- **Real-time:** live video streaming (RTMP ingest, FFmpeg, HLS) and WebRTC signalling in Go
- **Problem solving:** LeetCode Knight, top 2.71% in contest rating, 1000+ problems solved

Open to **remote senior backend roles**.

## What I'm building

### [LifeBoard](https://lifeboardos.com)

A journaling product: each day is a page of notes, photos, quotes and tasks, and every page becomes one square in a map of your whole life. NestJS and MongoDB on Cloud Run, with an Angular PWA client.

The backend work I'd point to:

- **Per-user envelope encryption.** AES-256-GCM data keys wrapped by Cloud KMS, ciphertexts bound to owner and field, rolled out in reversible stages with an idempotent backfill and a verification script.
- **Media migration without downtime.** Moved images from base64 inside MongoDB documents to Cloud Storage with signed links, quotas and an orphan sweep.
- **Reminders on a scale-to-zero platform.** Cloud Scheduler triggers an OIDC-guarded sweep endpoint, with graceful shutdown so a deploy never loses an in-flight push.
- **Hardened auth.** Hashed OTPs and refresh tokens, per-account lockout, per-endpoint rate limits.

## Selected work

| | |
|---|---|
| **Workflow engine** | Configuration-driven engine for a multi-stage loan pipeline; business teams change stage flows and validation rules without a release |
| **Underwriting engine** | Concurrent state transitions across multi-stage approvals, with isolated transactions for ACID guarantees |
| **Event-driven services** | NestJS and GCP Pub/Sub workers replacing manual credit-verification steps |
| **Live streaming server** | Go, goroutine-per-stream with channel-based fan-out, RTMP to HLS |
| **AR filter pipeline** | On-device inference with native C++ and MediaPipe, bridged to React Native |

## Stack

**Languages:** Go, TypeScript, C++, SQL
**Backend:** NestJS, Node.js, WebSockets, WebRTC, event-driven architecture
**Data:** PostgreSQL, SQL Server, MongoDB, Redis
**Infrastructure:** GCP (Cloud Run, Pub/Sub, KMS, Cloud Storage), Docker, GitHub Actions

## Find me

[Website](https://himanshusehlangia.dev) · [LinkedIn](https://linkedin.com/in/himanshu82817) · [LeetCode](https://leetcode.com/u/himanshu82817)
