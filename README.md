# Doğukan Tunçbilek

Senior software engineer. Curious about anything new, and the kind of person who loses sleep over a bug until it is understood.

```asm
xor   sleep, sleep
mov   ecx, coffee
rep   call analyze

; exit code: 0xC0FFEE
```

I build, extend and keep business systems running in production.

**What I do**

- .NET and SQL Server systems that have been in production for years: bugs, performance, upgrades, migrations. 5+ years on a custom enterprise ERP platform (.NET Framework 4.8, ASP.NET WebForms, a 30,000+ stored-procedure SQL Server database, SSRS/SSIS) serving 2,000+ dealers.
- Modern .NET: .NET 8/10, ASP.NET Core, EF Core, PostgreSQL, Redis/HybridCache, Docker, Helm/ArgoCD.
- Integrations: REST/SOAP, ERP (Logo, Netsis, Mikro, Nebim, 1C), e-invoice, payment and SMS gateways.
- IoT and mobile: Kotlin + RxAndroidBle companion apps, UART production-line test tooling, event-driven telemetry backends (Node/TypeScript, RabbitMQ, Redis, gRPC), React Native.
- Small-team DevOps: k3s on Hetzner bare-metal, OpenTofu, ArgoCD, GitHub Actions, WireGuard, Nginx.

**Repositories worth looking at** (small, focused, written from scratch with open-source libraries; each has tests and CI)

| Repo | What it does |
|---|---|
| [pdf-anchor-stamp](https://github.com/dogukantuncbilek/pdf-anchor-stamp) | Find a text marker inside a PDF (visible or invisible) and stamp an image or text at that exact spot. .NET 8, PdfPig + PDFsharp, CLI + library, tests. |
| [hetzner-k3s-gitops-starter](https://github.com/dogukantuncbilek/hetzner-k3s-gitops-starter) | One Hetzner server, k3s, Argo CD app-of-apps, cert-manager, Sealed Secrets, CloudNativePG, kube-prometheus-stack. Rebuild from zero in 15 minutes. |
| [receipt-ocr](https://github.com/dogukantuncbilek/receipt-ocr) | Receipt photos to JSON: OpenCV preprocessing (bilateral, CLAHE, adaptive thresholds), competing Tesseract strategies ranked by confidence, field extraction. FastAPI + Vue 3. |
| [hybridcache-redis-tags](https://github.com/dogukantuncbilek/hybridcache-redis-tags) | .NET 10 HybridCache + Redis: tag-based invalidation that crosses instances, stampede protection, readiness check. Runnable sample with two-instance tests. |
| [roslyn-remote-scripts](https://github.com/dogukantuncbilek/roslyn-remote-scripts) | Fetch C# scripts from a TypeScript script server, compile them at runtime with Roslyn inside a collectible AssemblyLoadContext, run them against a host API with hash-based caching and compile diagnostics. .NET 11 + TypeScript, tests and CI. |

**Selected work** (anonymised; details and images on [dogukantuncbilek.github.io](https://dogukantuncbilek.github.io))

- Digital approval workflow for work-order documents in an enterprise ERP (client under NDA): invisible report markers, PDF text search, approval seal drawn at the exact spot, GUID-registered documents, SMS/e-mail/push with one-time verify links, replay protection; 9 stored procedures, 2 TVPs, test suite 34 → 179. The stamping step lives on as [pdf-anchor-stamp](https://github.com/dogukantuncbilek/pdf-anchor-stamp).
- Marker-anchored PDF stamping library and CLI for .NET 8: [pdf-anchor-stamp](https://github.com/dogukantuncbilek/pdf-anchor-stamp).
- Cross-instance cache invalidation with .NET 10 HybridCache, Redis tags and a pub/sub bridge, proven by a two-instance test: [hybridcache-redis-tags](https://github.com/dogukantuncbilek/hybridcache-redis-tags).
- Single-server GitOps platform on Hetzner (OpenTofu, k3s, Argo CD, cert-manager, Sealed Secrets, CloudNativePG, Prometheus), rebuilt from zero in 15 minutes: [hetzner-k3s-gitops-starter](https://github.com/dogukantuncbilek/hetzner-k3s-gitops-starter).
- Thermal receipt OCR with OpenCV preprocessing and competing Tesseract strategies, FastAPI + Vue 3: [receipt-ocr](https://github.com/dogukantuncbilek/receipt-ocr).
- Remote C# scripting for long-running .NET hosts: scripts served by a TypeScript server, compiled at runtime with Roslyn into a collectible AssemblyLoadContext, cached by source hash, checked against a forbidden-API policy before compilation, re-fetched on ETag change; .NET 11 engine and console host, Fastify server, 19 xUnit + 13 vitest tests: [roslyn-remote-scripts](https://github.com/dogukantuncbilek/roslyn-remote-scripts).

**How I work:** read the existing code first, explain the root cause before changing anything, keep changes small and tested, write down what I did.

**Find me on:** [Portfolio](https://dogukantuncbilek.github.io) · [Upwork](https://www.upwork.com/freelancers/dogukantuncbilek) · [LinkedIn](https://www.linkedin.com/in/dogukan-tuncbilek)
