<div align="center">
  <h1>Faycal Rafa</h1>
  <h3>Senior Software Engineer • Technical Lead & Systems Architect</h3>
  <p>
    <em>6+ years architecting fault-tolerant microservices, enterprise SaaS platforms, and flagship native Android applications across Fintech, Automotive, and High-Traffic Consumer ecosystems.</em>
  </p>

  <p>
    <a href="[https://faycalrafa.github.io](https://faycalrafa.github.io)"><strong>🌐 Live Portfolio & Architecture Case Studies</strong></a> •
    <a href="[https://faycalrafa.github.io/projects](https://faycalrafa.github.io/projects)"><strong>📂 Verified Project Proofs</strong></a> •
    <a href="[https://faycalrafa.github.io/Faycal_Rafa_CV_2026.pdf](https://faycalrafa.github.io/Faycal_Rafa_CV_2026.pdf)"><strong>📄 Download CV (PDF)</strong></a> •
    <a href="[https://wa.me/213540980238](https://wa.me/213540980238)"><strong>💬 Direct Contact</strong></a>
  </p>
</div>

---

### 🏛️ Architectural Domains & Core Stack

| Domain | Core Technologies & Production Capabilities |
| :--- | :--- |
| **Distributed Backend & Microservices** | **NestJS**, **Node.js**, **TypeScript (Strict)**, **Laravel (PHP 8+)**, **Python** — *Monolith-to-microservice decomposition, event-driven WebSockets, idempotent fintech transaction flows, high-concurrency REST/GraphQL APIs.* |
| **Native & Cross-Platform Mobile** | **Android Native (Kotlin/Java)**, **Jetpack Compose (M3)**, **AndroidX Media3 (ExoPlayer)**, **Flutter/Dart** — *Offline-first storage engines, custom multi-engine TTS pipelines, lockscreen `MediaSessionService`, real-time GPS telemetry.* |
| **Data, DevOps & Infrastructure** | **PostgreSQL (Partitioning/JSONB)**, **MySQL**, **MongoDB**, **Docker (Multi-Stage)**, **Linux Administration**, **GitHub Actions** — *ERD normalization, reverse-proxy hardening, zero-downtime CI/CD automation, local LLM/RAG inference workflows.* |
| **Modern Reactive Frontend** | **Next.js (App Router)**, **Svelte 5 (Runes)**, **React**, **Astro 5**, **Tailwind CSS v4** — *Type-safe domain modeling, Web Speech/AudioContext APIs, high-performance enterprise dashboards.* |

---

### 🚀 Flagship Engineering & System Proofs

> *Note: Several enterprise platforms (Fintech, B2B Automotive SaaS, and Digital Wallets) live in private organization repositories. Full architectural deep-dives, ERDs, and live interactive demos are available on my [Portfolio](https://faycalrafa.github.io/projects).*

| System / Project | Architecture & Stack | Engineering Highlight |
| :--- | :--- | :--- |
| **[BookReader Flagship](https://faycalrafa.github.io/projects/bookreader)** | `Kotlin` `Jetpack Compose M3` `Media3` `Jsoup` | Offline-first Android novel reader with quote-aware multi-engine TTS segmentation, `AtomicFile` mutex storage, and zero-thread-collision `MediaSessionService` background audio. |
| **[SABIL Mega-App](https://faycalrafa.github.io/projects#sabil)** | `Microservices` `NestJS` `PostgreSQL` `Docker` | High-availability digital wallet & multi-service consumer platform with resilient multi-channel payment transaction pipelines. |
| **[InvestMarket Platform](https://faycalrafa.github.io/projects#investmarket)** | `NestJS` `Next.js` `TypeScript` `Docker` | Full-stack enterprise investment platform built on decoupled microservice transports and strict end-to-end type validation. |
| **[AUTOQUAL & PIASSA SaaS](https://faycalrafa.github.io/projects#piassa)** | `TypeScript` `Laravel` `MySQL` `Docker` | Enterprise automotive CRM, multi-warehouse inventory synchronization, and high-throughput B2B/B2C parts cataloging. |
| **[StartingPack](https://faycalrafa.github.io/projects#startingpack)** | `Svelte 5 (Runes)` `TypeScript` `Tailwind v4` | Reactive micro-application showcasing fine-grained `$state`/`$derived` reactivity and zero-runtime-overhead UI state. |

---

### 🔄 How I Architect Systems (Reference Topology)

```mermaid
flowchart LR
    subgraph Clients["Client Layer"]
        A["Android Native\n(Compose M3 / Media3)"]
        B["Enterprise Web\n(Next.js / Svelte 5)"]
    end

    subgraph Edge["Gateway & Security"]
        C["Reverse Proxy & API Gateway\n(Rate Limiting / JWT / TLS)"]
    end

    subgraph Core["Distributed Services"]
        D["Domain Microservices\n(NestJS / Node.js / Laravel)"]
        E["Async Workers & Event Bus\n(Queues / WebSockets)"]
    end

    subgraph Data["Persistence & Infra"]
        F[("PostgreSQL / MySQL\n(Partitioned & Indexed)")]
        G["Dockerized Linux Nodes\n(Automated CI/CD)"]
    end

    A & B --> C --> D
    D <--> E
    D & E --> F
    G -.->|Orchestrates| D & E
