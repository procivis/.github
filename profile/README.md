Procivis One is a modular system for digital identity and credentials.
This page covers how the system is composed and what each component does.

## Architecture

![Procivis One Core - Architecture](/profile/Procivis_One_Architecture.png)

The architecture diagram shows the full system: the open source Core at
the foundation, the components built on top of it, and the integration
interfaces (REST API, SDK, and mobile SDK) that connect them to external
systems and applications.

## Components
 
Procivis One is made up of five components: Core, Desk, Wallet-Relying
Party Registry, Mobile, and OpenID Bridge.

### Core

<img width="1096" height="939" alt="Core Component" src="https://github.com/user-attachments/assets/708d7684-f496-49bc-91ee-8a4004451abb" />

The Procivis One Core is the open source foundation of the system. It
integrates into applications via REST API, server SDK, or mobile SDK
(React Native, Swift, Kotlin).

Core capabilities include:

- **Credential lifecycle** — issue, hold, verify, revoke, and suspend
  credentials across all supported formats and identifiers
- **Certificate management** — generate certificate authorities, issue
  and sign certificates, and manage revocation via CRL, without external
  PKI infrastructure
- **Wallet provider** — issue wallet unit attestations (WUA), wallet
  instance attestations (WIA), and manage trust list collections for
  wallets
- **Trusted list publishing** — publish and manage trusted lists in
  supported formats

See [Standards]([/standards](https://docs.procivis.ch/standards)) for the current
list of supported technologies and protocols.

[Procivis One Core on GitHub](https://github.com/procivis/one-core) ·
[Core API reference](https://docs.procivis.ch/reference/core/procivis-one-core-api)

### Desk

<img width="862" height="740" alt="component_desk" src="https://github.com/user-attachments/assets/d1b0d1a9-3d2b-4f31-9951-14b52f37344a" />

Desk is the enterprise backend component. It wraps the Core with
functionality designed for organizational deployments. Desk capabilities
include:

- **IAM integration** — integrate with your existing identity provider with
  streamlined OpenID Connect token exchange and role-to-permission mapping
- **Multi-tenant organization management** — run multiple organizations and
  manage their resources independently within a single deployment
- **Country profiles** — pre-configured credential format and protocol
  settings for supported national ecosystems, simplifying compliance for
  users
- **Desk UI** — a no-code web interface for managing the full capabilities
  of Core, Desk, WRPR, and OpenID Bridge

[Desk API reference](https://docs.procivis.ch/reference/desk/procivis-one-desk-api) ·
[Try the Desk UI](https://docs.procivis.ch/trial)

### Wallet-Relying Party Registry

<img width="886" height="692" alt="component_wrpr" src="https://github.com/user-attachments/assets/a2df6c5c-63ad-4f42-824a-5b05b4e73f63" />

The Wallet-Relying Party Registry (WRPR) is infrastructure for national
wallet-relying party registration schemes. It handles registrar functions
for national registry compliance (EU 2025/848, ETSI TS 119 475, ETSI TS 119
411-8) and certificate provisioning (access certificates and registration
certificates). The WRPR service runs on Core and can be operated standalone
or together with Desk — when deployed with Desk, the Desk UI provides the
registrar interface with the enterprise backend benefits of Desk.
 
[Wallet-Relying Party Registry](https://docs.procivis.ch/wallet-relying-party-registry) ·
[WRPR API reference](https://docs.procivis.ch/reference/wrpr/wallet-relying-party-registry-api)

### Mobile
 
The Mobile component covers two applications built on the Core's mobile SDK:
 
**Wallet App** — a digital wallet for holding and presenting credentials.
Available as an open source reference implementation that can be
white-labelled, or embedded into an existing app using the One Core React
Native SDK and React Native Components library.
 
**Verifier App** — an enterprise mobile verifying application supporting
offline verification over Bluetooth Low Energy (BLE) in both OID4VP and ISO
mdoc flows. The app is available on app stores and can be initialized in our
[trial environment](/trial) for testing and demonstration.
 
[Procivis One Wallet on GitHub](https://github.com/procivis/one-wallet) ·
[React Native SDK on GitHub](https://github.com/procivis/react-native-one-core) ·
[SDK documentation](https://docs.procivis.ch/reference/sdk)

### OpenID Bridge
 
The OpenID Bridge integrates verifiable credentials into existing IAM
systems, enabling credential-based login for any OIDC provider without
replacing existing infrastructure. Available under an enterprise license.
 
[OpenID Bridge documentation](https://docs.procivis.ch/openid-bridge)

## Licensing
 
| Open source | Enterprise |
|---|---|
| Procivis One Core | Procivis One Desk |
| Procivis One Wallet App | Procivis One Verifier App |
| One Core React Native SDK | Procivis One Business Wallet |
| One React Native Components | Wallet-Relying Party Registry |
| | OpenID Bridge |
 
[Procivis on GitHub](https://github.com/procivis) ·
[Contact us](https://www.procivis.ch/en/contact) for enterprise licensing
