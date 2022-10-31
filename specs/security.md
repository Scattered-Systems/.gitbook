---
description: Discussing the implementation and viability of post-quantum protocols
---

# Security

In order for our systems to achieve a quantum resilient architecture, it is imperative to question the very nature of each technology at play to discover their faults and explorer their engines.

One method we are currently implementing was recently formalized by researchers at IOHK with their tweakable sleeve. A tweakable sleeve implements a more modular novel sleeve mechanism leveraging a composition derived from a tweakable hash function. The beauty of the technology is the intended use case, as the protocol was designed to imbue quantum-resilience upon naturally non-quantum elliptic curve cryptographic protocols.

