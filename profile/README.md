# VIEApps NGX

**The Communication Runtime for Distributed Systems**

Decouple service logic from system operation. Control distributed execution at runtime — not through infrastructure.

![VIEApps NGX Architecture](https://fs.vieapps.net/images/e7d874add436487ba0d092e5d5246d6b/ef1bce6dc66f418e8df5a6ed631c13d3/vieapps-ngx-architecture.png.webp)

### What is this?

A unified runtime that replaces your service mesh, API gateway, RPC framework, and most your YAML files.

Core ideas:

- **Routed RPC**: Services don't call each other. The runtime routes.

- **Admission Control**: Concurrency in slots. Your CPU metrics are lying to you.

  *Reference: Ubuntu 24.04, 4 vCPU/8GB = 1,500 slots/node. 

  2019 baseline: 2 vCPU/4GB = ~900 slots at 20k ops/s. 

  Tune based on your Router node's actual throughput.*

- **Transport Agnostic**: REST, WebSocket, SSE, MCP - same execution model.

- **Runtime-Aware Edge**: Cache invalidation by business logic, not TTL guesswork.

### Who is this for?

**Not for you if**: You've never run distributed systems in production.
VIEApps NGX assumes you understand why "microservices" became "microservice hell".

**For you if**: You've paid the K8s tax. You've been bitten by service mesh latency.
You've watched a single slow service take down your entire cluster.
You know infrastructure shouldn't be your product.

By moving control from service code and infrastructure layers into a unified runtime, VIEApps NGX enables scalable, resilient, and loosely coupled system architectures.

This is not middleware. This is your system's nervous system.

### Latest battle-tested
May 7, 2026 - National traffic spike:
- 3,278 concurrent requests
- 1.15M requests in 60 minutes  
- 0 rejections, 0 nodes scaled
- 36% capacity used

The runtime applied backpressure when Redis choked. No circuit breakers fired.
Because we don't do circuit breakers. We do admission control.

### The Hard Truth

**The code is free. The expertise isn't.**

VIEApps NGX is open-source. You can clone it right now.

But if you don't understand:

- Why WAMP with Routed RPC instead of gRPC

- Why ReactiveX for execution pipelines

- Why slots instead of CPU thresholds

- Why admission control beats auto-scaling

...then you'll deploy it wrong. And blame the tool.

We've been running this in production since 2017. 
We learned these lessons so you don't have to.

### Get Started

**Code**: https://github.com/vieapps

**Docs**: https://vieapps.com

**Commercial Support**: For when you realize free code doesn't mean free operations

### License
Apache 2.0. Use it. Fork it. But if you go to production with it, talk to someone who's been there.

---
*If K8s was your first distributed system, VIEApps NGX is your last.*
