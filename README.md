# Doğukan Tunçbilek

Senior software engineer. Curious about anything new, and the kind of person who loses sleep over a bug until it is understood.

```asm
xor   sleep, sleep      ; sleep = 0
mov   ecx, coffee
rep   call analyze
; exit code: 0xC0FFEE
```

I fix, extend and ship software that other people are afraid to touch.

**What I do**

- .NET and SQL Server systems that have been in production for years: bugs, performance, upgrades, migrations. 5+ years on a custom enterprise ERP platform (.NET Framework 4.8, ASP.NET WebForms, a 30,000+ stored-procedure SQL Server database, SSRS/SSIS) serving 2,000+ dealers.
- Modern .NET: .NET 8/10, ASP.NET Core, EF Core, PostgreSQL, Redis/HybridCache, Docker, Helm/ArgoCD.
- Integrations: REST/SOAP, ERP (Logo, Netsis, Mikro, Nebim, 1C), e-invoice, payment and SMS gateways.
- IoT and mobile: Kotlin + RxAndroidBle companion apps, UART production-line test tooling, event-driven telemetry backends (Node/TypeScript, RabbitMQ, Redis, gRPC), React Native.
- Small-team DevOps: k3s on Hetzner bare-metal, OpenTofu, ArgoCD, GitHub Actions, WireGuard, Nginx.

**Repositories worth looking at** (small, focused, rewritten from scratch with open-source libraries)

| Repo | What it does |
|---|---|
| `pdf-anchor-stamp` | Find a text marker inside a PDF and stamp an image or text at that exact spot. .NET 8, PdfPig + PDFsharp. *(in progress)* |
| `hetzner-k3s-gitops-starter` | OpenTofu → Hetzner → k3s → ArgoCD app-of-apps with cert-manager, Sealed Secrets, CloudNativePG and monitoring. *(planned)* |
| `receipt-ocr` | Receipt OCR with OpenCV preprocessing and Tesseract/EasyOCR, Vue 3 front end. *(planned)* |
| `hybridcache-redis-tags` | .NET 10 HybridCache + Redis with tag-based invalidation and health checks. *(planned)* |

**How I work:** read the existing code first, explain the root cause before changing anything, keep changes small and tested, write down what I did.

Available for contract and freelance work. Upwork: [upwork.com/freelancers/dogukantuncbilek](https://www.upwork.com/freelancers/dogukantuncbilek)
