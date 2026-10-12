# Awesome-Enterprise-Cloud-Encryption

## Top Enterprise Cloud Encryption Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Data-at-Rest Encryption, Key Management & Cloud Data Protection*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Cloud Encryption**. These tools help organizations protect sensitive data at rest across cloud applications, databases, and storage systems — with customer-controlled keys, field-level encryption, and compliance-ready audit trails.



**Examples** include Salesforce Platform Encryption, HashiCorp Vault, AWS KMS, Azure Key Vault, Google Cloud KMS, CipherCloud, Baffle, Protegrity, Thales CipherTrust, and Townsend Security (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, envelope encryption, and open key management — ideal for security engineers, compliance teams, and developers seeking transparent, vendor-independent cloud encryption.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Salesforce Platform Encryption](https://help.salesforce.com/s/articleView?id=platform.shield_ext_pe_analyzer.htm&type=5)**  

  Native Salesforce field-level encryption using AES-256 symmetric keys. Features Platform Encryption Analyzer to identify encryptable fields, Bring Your Own Key (BYOK) via HSM or external key service, key rotation, and Data Cloud key management. Protects PII and PHI while preserving search, workflow, and validation rules .



- **[HashiCorp Vault](https://www.hashicorp.com/)**  

  Industry-standard secrets and key management platform. Features transit engine for encryption-as-a-service, PKI, dynamic secrets, and HSM integration. Available as self-hosted or HCP managed cloud.



- **[AWS KMS](https://aws.amazon.com/kms/)**  

  Native AWS key management with envelope encryption for virtually every AWS service. Features multi-Region keys, XKS (HYOK) for external key control, CloudHSM, and CloudTrail audit logging.



- **[Azure Key Vault](https://azure.microsoft.com/en-us/products/key-vault/)**  

  Azure's native key, secret, and certificate service. Features Managed HSM tier (FIPS 140-2 Level 3), Entra RBAC, automatic rotation, and per-operation pricing.



- **[Google Cloud KMS](https://cloud.google.com/security-key-management)**  

  GCP's native key management with Cloud EKM (External Key Manager) for keys residing outside Google. Features Cloud HSM, CMEK across GCP services, and key-justification logging.



- **[CipherCloud](https://www.ciphercloud.com/)**  

  Cloud access security broker with encryption and tokenization for SaaS applications. Protects data in Salesforce, Microsoft 365, and other cloud apps.



- **[Baffle](https://baffle.io/)**  

  Data protection platform with field-level encryption and tokenization for cloud databases. Features no-code deployment and format-preserving encryption.



- **[Protegrity](https://www.protegrity.com/)**  

  Enterprise data security platform with encryption, tokenization, and data masking. Protects data across cloud, on-prem, and hybrid environments.



- **[Thales CipherTrust](https://cpl.thalesgroup.com/)**  

  Enterprise key management and data protection platform. Features centralized key lifecycle, HSM integration, database encryption, and multi-cloud key orchestration.



- **[Townsend Security](https://www.townsendsecurity.com/)**  

  Encryption and key management solutions for enterprise compliance. Features Alliance Key Manager and database encryption for SQL Server, Oracle, and cloud databases.



## Open-Source GitHub Projects



- **[RustyVault](https://github.com/Tongsuo-Project/RustyVault)**  

  Modern secret management system in Rust (Apache-2.0) designed as a seamless HashiCorp Vault replacement. Features OSI-approved license, configurable cryptographic modules (OpenSSL, Tongsuo, native Rust), RESTful API compatible with Vault, PKI/CA infrastructure with RSA/ECC/SM2 support, key management (symmetric/public), and active/active clustering. Supports AES/SM4 encryption, RSA/ECDSA/EdDSA/SM2 signatures, and Paillier EC-ElGamal for cryptographic computing .



- **[HyperionDB Vault](https://crates.io/crates/hyperion-vault)**  

  Self-contained, replicated secrets vault in Rust (license varies). Features envelope encryption with AWS KMS-wrapped DEKs, XChaCha20-Poly1305 sealed secrets, embedded redb storage, Raft replication for high availability, IP allowlist for reads, RBAC with path globs, brute-force lockout, KMS-outage resilience with DEK caching, and audit log. Only ciphertext, wrapped DEK, and nonce ever written to disk .



- **[Nexus](https://github.com/ConstantineCTF/nexus)**  

  Enterprise-grade secrets management with encryption, versioning, and backup (MIT). Features immutable Ed25519-signed logs, version history for SOC 2 compliance, RBAC support, compliance reports, one-command encrypted backups (AES-256-GCM), point-in-time recovery, and single-binary deployment. REST API and Go SDK included .



- **[secrets (Go)](https://pkg.go.dev/github.com/allisson/secrets)**  

  Lightweight secrets manager in Go (MIT) inspired by HashiCorp Vault but intentionally simpler. Features envelope encryption, transit encryption (EaaS), tokenization engine for format-preserving tokens, token-based auth with Argon2id, native KMS integration (GCP, AWS, Azure, Vault), PostgreSQL backend, and OpenTelemetry metrics. Not yet recommended for production at v0.x .



- **[PyHSM](https://pypi.org/project/vectorguard-pyhsm/)**  

  Software HSM core in Python (license varies). Features AES-256-GCM outer envelope with HMAC-SHA256 tamper seal, AES-KWP per-key wrapping, policy engine (ACL, rate, expiry, ops), audit logging with HMAC-chained append-only logs, key zeroization from memory, and persistent keystore. Supports secp256k1, ed25519, and AES-256 key types .



- **[Age](https://github.com/FiloSottile/age)**  

  Simple, modern file encryption tool (BSD-3-Clause). Features small explicit keys, no config options, and UNIX-style composability. Widely used for encrypting secrets in GitOps workflows and backup pipelines .



- **[SOPS](https://github.com/getsops/sops)**  

  Secrets encryption tool for configuration files (MPL-2.0). Structure-preserving encryption keeps file format intact while encrypting values. Integrates with AWS KMS, GCP KMS, Azure Key Vault, and age. Widely used for GitOps secret management .



- **[Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets)**  

  Kubernetes secret encryption for GitOps (Apache-2.0). Encrypts secrets with a public key so they can be safely stored in public version control. Only the cluster's private key can decrypt. Features key rotation and offline recovery .



- **[External Secrets Operator](https://github.com/external-secrets/external-secrets)**  

  Kubernetes operator integrating external secret managers (Apache-2.0). Syncs secrets from AWS Secrets Manager, HashiCorp Vault, Google Secret Manager, Azure Key Vault, and more into native Kubernetes Secrets .



### Additional Strong Open-Source Options



- **[OpenBao](https://github.com/openbao/openbao)** — Community fork of HashiCorp Vault under MPL 2.0, maintained by Linux Foundation.

- **[Infisical](https://github.com/Infisical/infisical)** — Open-source secrets, certificates, and privileged access management platform (MIT for core).

- **[Cosmian KMS](https://github.com/Cosmian/kms)** — Pure Rust KMIP 1.4-compliant key management system with FIPS 140-3 compliance.

- **[Clef](https://github.com/clef-sh/clef)** — Tokenless secrets manager running on Git and cloud KMS (MIT).

- **[gopass](https://github.com/gopasspw/gopass)** — Terminal-based password manager using GPG and Git (MIT) .

- Community **n8n** workflows for encryption key rotation automation and compliance alerting.



**Frameworks for building custom systems**: Combine **RustyVault** or **OpenBao** as the secrets management core with **SOPS** for GitOps-encrypted configuration, **Sealed Secrets** or **External Secrets Operator** for Kubernetes-native delivery, **HyperionDB Vault** for replicated vault clusters, and **PostgreSQL** for persistence — creating a fully self-hosted, enterprise-grade cloud encryption platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud encryption systems handling cryptographic material must comply with security standards (FIPS 140-2/3, SOC 2, PCI-DSS, HIPAA, etc.).

- Self-hosted open-source solutions require proper security hardening, HSM integration where required, and ongoing maintenance. Key custody is a security-critical operation demanding appropriate operational expertise.



---



**Made for security engineers, compliance officers, platform teams, and developers building transparent cloud encryption solutions.**  

Let's make Enterprise Cloud Encryption more open, secure, and interoperable.
