# VIEApps NGX

![VIEApps NGX: Clean Architecture - Pure Performance](https://fs.vieapps.net/images/e7d874add436487ba0d092e5d5246d6b/ef1bce6dc66f418e8df5a6ed631c13d3/vieapps-ngx-architecture.png.webp)

A platform for communication, routing, and execution in distributed systems

Decouple service logic from system operation.

Control distributed execution at runtime — not through infrastructure.

### Move control from infrastructure to runtime

VIEApps NGX introduces an application-level runtime that manages:

- message-driven service communication
- routed RPC execution across nodes
- dynamic load distribution and coordination

This eliminates direct coupling between services and reduces reliance on infrastructure-level mechanisms such as service mesh or tightly bound RPC layers.

### One runtime, multiple communication patterns

- REST for request-response
- WebSocket for bidirectional real-time
- SSE as fallback under network constraints
- MCP for AI-native integration via Model Context Protocol, exposing Routed RPC as tools/resources

All mapped into the same internal execution model.

### Built for real-world load

Runtime-level admission control regulates concurrency and request flow, ensuring:

- stability under traffic spikes
- protection against overload
- consistent system responsiveness

### Choose your perspective

[ [For Business](https://vieapps.com/ngx/what-is-vieapps-ngx/for-business.html) ]

Scale systems without re-architecture — even under real-world load.

[ [For Engineering](https://vieapps.com/ngx/what-is-vieapps-ngx/for-engineering.html) ]

Understand how communication, routing, and execution are controlled at runtime.

### Deep dive

Full architecture, execution model, and design principles:

→ [What is VIEApps NGX, really?](https://vieapps.com/ngx/what-is-vieapps-ngx/what-really-vieapps-ngx-is.html)
