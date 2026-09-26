# Production Auth Service

> A production-ready authentication microservice designed for distributed systems, bridging high-performance stateless access with strict, stateful session control.

This service implements a highly resilient dual-token architecture optimized for scale. It handles stateless access tokens (JWTs) for low-latency authorization, alongside stateful refresh token rotation with cryptographic reuse detection to neutralize replay attacks.

## Capabilities
* **Stateless Access Verification:** Enables downstream microservices to verify authorization instantly without database hits.
* **Stateful Token Rotation:** Secures long-lived sessions by rotating refresh tokens and invalidating compromised token families.
* **Active Session Management:** Tracks session origins, allowing for granular device logouts or global session revocation.
