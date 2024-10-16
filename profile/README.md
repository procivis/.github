# Procivis One

Procivis One is a robust solution capable of powering every element of the digital identity
credential lifecycle — schema definition, credential design, issuance, holding, revocation,
suspension, updating and verifying digital credentials — and integrating them into business
processes through a range of integration pathways and deployments.

Handle credential-driven use cases and processes flexibly with an extensible configuration
that supports multiple credential formats, revocation methods, key types, signatures, and
DID methods. Procivis One is built to connect your organization to the SSI ecosystem, become
compatible with regulations such as **eIDAS 2.0**, and be extensible as new regulations and
requirements emerge.

## Key features

- **Interoperable**
  - Uses standardized protocols for credential lifecycles for maximum compatability with
    software from other vendors. See the results of [interoperability][interop]
    testing.
- **Flexible**
  - Supports a wide range of credential formats, interaction protocols and trust infrastructures,
    with more being added as standardization processes mature and regulatory requirements develop.
    This includes all standards within the [**eIDAS 2.0 regulation**][eidas], the
    **Swiss eID infrastructure**, and more. See the [supported standards][suppstand].
- **End-to-end**
  - Provides the infrastructure and tooling for every stakeholder in the digital identity
    and credential lifecycle — issuer, holder and verifier — via the powerful API, wherever
    it is installed and deployed.
- **Private**
  - Enables a high level of privacy for all stakeholders with decentralized data storage,
    selective disclosure, privacy-preserving revocation and many more privacy-focused features.
- **Performant**
  - Built with Rust to power all aspects of the digital identity and credential lifecycle
    with maximum efficiency, allowing you to reliably scale to millions of credential lifecycle
    events with ease.
- **Deployable**
  - Can be deployed wherever you need digital identity and credential capabilities, from
    large data centers or cloud providers to smart devices and IoT; the same code base can
    be used for server components and for mobile apps via the SDK.

## Architecture

![Procivis One Core - Architecture](/architecture_one_core.png)

Use the Procivis One Core to build components for your own use case, or use one of the
existing components built on the Core.

### Open source

- **Procivis One Core**: handles everything needed to
    issue, hold and verify decentralized digital identity and credentials, and integrates into
    business and IT applications via REST, SDK, or mobile SDK. Use the Procivis One Core to build components
    for your own use case, or use one of the existing components built on the Core.
        - [Procivis One Core][core]
- **Procivis One Wallet**: a digital wallet solution that includes the SSI functionality
    of the Core and is available with an open source license. Use the Procivis One Wallet
    for a free-standing solution that can be white-labelled, use the React Native One Core
    to embed wallet capabilities into an existing app, and use the One React Native Components library
    for UI elements for your digital wallet app.
        - [Procivis One Wallet][wallet]
        - [React Native One Core][rncore]
        - [One React Native Components][comp]

### Enterprise

- **Procivis One Desk**: a server-based solution that includes the SSI functionality
    of the Core and adds enterprise functionality such as user and session management, and a
    dashboard for no-code issuance and verification. [Sign up for the trial][trial].
- **Procivis One Mobile Verifier**: a mobile verifying solution that includes the SSI
    functionality of the Core and enables offline verification in both OID4VP and ISO mdoc flows
    over Bluetooth Low Energy (BLE). See the trial version in the iOS and Android app stores.

### Components

The following graphic represents a **component view** of Procivis One. All components
are built from the Procivis One Core and share the same code base.

![Procivis One Components](/Procivis_One_components.png)

[Contact us][contact] to find out more.

[comp]: https://github.com/procivis/one-react-native-components
[contact]: https://www.procivis.ch/en/contact
[core]: https://github.com/procivis/one-core
[eidas]: https://github.com/procivis/one-core?tab=readme-ov-file#eidas-20
[interop]: https://github.com/procivis/one-core?tab=readme-ov-file#interoperability-and-conformance
[rncore]: https://github.com/procivis/react-native-one-core
[suppstand]: https://github.com/procivis/one-core?tab=readme-ov-file#supported-standards
[trial]: https://docs.procivis.ch/trial/intro
[wallet]: https://github.com/procivis/one-wallet
