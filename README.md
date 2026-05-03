# Zero Trust Architecture (zero-trust-architecture)

Zero Trust Architecture (ZTA) is a security framework defined by NIST SP 800-207 that requires all users and devices to be authenticated, authorized, and continuously validated before being granted access to applications and data, regardless of whether they are inside or outside the network perimeter. The architecture is built on the principle of "never trust, always verify," replacing implicit trust with explicit verification for every access request.

**URL:** [https://www.nist.gov/publications/zero-trust-architecture](https://www.nist.gov/publications/zero-trust-architecture)

## Tags:

 - Access Control, Authentication, Authorization, Cybersecurity, Identity Management, Least Privilege, Network Security, NIST, Security, Zero Trust

## Timestamps

- **Created:** 2025
- **Modified:** 2026-05-03

## APIs

### NIST SP 800-207 Zero Trust Architecture

NIST Special Publication 800-207 defines zero trust architecture and provides a roadmap for organizations migrating to ZTA. It describes seven ZTA tenets, three logical components (PDP, PEP, PAP), three ZTA deployment approaches, and guidance on threat models. Published August 2020.

- [Documentation](https://csrc.nist.gov/pubs/sp/800/207/final)
- [Specification](https://nvlpubs.nist.gov/nistpubs/specialpublications/NIST.SP.800-207.pdf)

### NIST SP 800-207A ZTA for Cloud-Native Applications

Extends ZTA guidance to cloud-native applications in multi-cloud environments, addressing service mesh architectures, workload identity, microsegmentation, and API-centric access control patterns.

- [Documentation](https://csrc.nist.gov/pubs/sp/800/207/a/final)
- [Specification](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-207A.pdf)

### SPIFFE - Secure Production Identity Framework for Everyone

CNCF-graduated open standard for workload identity in dynamic environments, providing SPIFFE Verifiable Identity Documents (SVIDs) for mutual TLS authentication without static secrets.

- [Documentation](https://spiffe.io/docs/latest/)
- [GitHub](https://github.com/spiffe)

### SPIRE - SPIFFE Runtime Environment

Reference implementation of SPIFFE providing workload identity attestation across Kubernetes, VMs, cloud instances, and bare metal. CNCF-graduated project.

- [Documentation](https://spiffe.io/docs/latest/spire-about/)
- [GitHub](https://github.com/spiffe/spire)

### Open Policy Agent (OPA)

CNCF-graduated open source policy engine serving as the Policy Decision Point (PDP) in ZTA implementations, using the Rego language for context-aware access policy evaluation.

- [Documentation](https://www.openpolicyagent.org/docs/latest/)
- [GitHub](https://github.com/open-policy-agent)

## Common Properties

- [NIST SP 800-207 PDF](https://nvlpubs.nist.gov/nistpubs/specialpublications/NIST.SP.800-207.pdf)
- [NIST SP 800-207A PDF](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-207A.pdf)
- [CISA Zero Trust Maturity Model](https://www.cisa.gov/zero-trust-maturity-model)
- [NSA Zero Trust Guidance](https://www.nsa.gov/Press-Room/News-Highlights/Article/Article/2899282/nsa-releases-guidance-on-zero-trust-security-model/)
- [DoD Zero Trust Reference Architecture](https://dodcio.defense.gov/Portals/0/Documents/Library/ZT-Reference-Architecture.pdf)
- [SPIFFE Project](https://spiffe.io/)
- [Open Policy Agent](https://www.openpolicyagent.org/)

## Features

| Name | Description |
|------|-------------|
| Identity Verification | Every access request requires verification of user and device identity regardless of network location. |
| Least Privilege Access | Access is granted with minimum required permissions on a per-session basis. |
| Microsegmentation | Networks are divided into small zones to limit lateral movement after breach. |
| Continuous Monitoring | All network traffic, user behavior, and device health are continuously monitored and analyzed. |
| Policy Decision Point | Centralized policy engine evaluates access requests against defined policies. |
| Policy Enforcement Point | Gateway or proxy that enforces access decisions made by the policy engine. |
| Workload Identity | Cryptographic identity for workloads and services replacing static credentials. |
| Device Health Attestation | Device posture and compliance are verified before granting access. |
| Implicit Trust Elimination | No user, device, or network is trusted implicitly, even inside the corporate perimeter. |
| Multi-Factor Authentication | Strong MFA is required as part of identity verification for all access. |

## Use Cases

| Name | Description |
|------|-------------|
| Remote Workforce Security | Providing secure access to enterprise resources for remote employees without VPN. |
| Cloud Application Access | Controlling access to multi-cloud and SaaS applications with consistent policies. |
| API Security | Enforcing zero trust principles at API gateways with per-request authentication and authorization. |
| Kubernetes Workload Identity | Using SPIFFE/SPIRE to assign cryptographic identities to Kubernetes pods. |
| Supply Chain Security | Verifying identity and integrity of software components and build pipelines. |
| Government Compliance | Meeting CISA Zero Trust Maturity Model requirements for federal agencies. |
| Insider Threat Mitigation | Limiting damage from insider threats through continuous monitoring and least privilege. |
| Multi-Cloud Security | Applying consistent zero trust policies across AWS, Azure, GCP, and private clouds. |

## Integrations

| Name | Description |
|------|-------------|
| SPIFFE/SPIRE | Workload identity standard providing SVIDs for mutual TLS authentication. |
| Open Policy Agent | Policy engine serving as the Policy Decision Point in ZTA implementations. |
| Envoy Proxy | Service mesh proxy enforcing mTLS and authorization policies as PEP. |
| Istio | Kubernetes service mesh providing ZTA controls through SPIFFE and OPA integration. |
| HashiCorp Vault | Secrets management platform providing dynamic credentials in ZTA pipelines. |
| Okta | Identity provider for user and device authentication in ZTA implementations. |
| Microsoft Entra ID | Cloud identity platform used as Identity Provider in enterprise ZTA deployments. |
| BeyondCorp Enterprise | Google's ZTA implementation for context-aware access to enterprise applications. |
| Cloudflare Zero Trust | Zero Trust Network Access and secure web gateway platform. |
| Zscaler Private Access | Cloud-native ZTNA solution providing ZTA-compliant access to private applications. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [Zero Trust Policy Schema](json-schema/zero-trust-architecture-policy-schema.json)
- [Zero Trust Identity Schema](json-schema/zero-trust-architecture-identity-schema.json)
- [Zero Trust Resource Schema](json-schema/zero-trust-architecture-resource-schema.json)

### JSON Structure

- [Zero Trust Policy Structure](json-structure/zero-trust-architecture-policy-structure.json)
- [Zero Trust Identity Structure](json-structure/zero-trust-architecture-identity-structure.json)

### JSON-LD

- [Zero Trust Architecture JSON-LD Context](json-ld/zero-trust-architecture-context.jsonld)

### Examples

- [Zero Trust Policy Example](examples/zero-trust-architecture-policy-example.json)
- [Zero Trust Identity Example](examples/zero-trust-architecture-identity-example.json)

## Vocabulary

- [Zero Trust Architecture Vocabulary](vocabulary/zero-trust-architecture-vocabulary.yaml) — Unified taxonomy mapping 8 resources, 8 actions, 3 workflows, 6 personas, and 15 core concepts across the Zero Trust Architecture domain.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
