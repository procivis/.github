# Procivis One

*Procivis One* is a robust solution capable of powering every element of the digital identity
credential lifecycle — schema definition, credential design, issuance, holding, revocation,
suspension, updating and verifying digital credentials — and integrating them into business
processes through a range of integration pathways and deployments.

Handle credential-driven use cases and processes flexibly with an extensible configuration
that supports multiple credential formats, revocation methods, key types, signatures, and
DID methods. *Procivis One* is built to connect your organization to the SSI ecosystem, become
compatible with regulations such as **eIDAS 2.0**, and be extensible as new regulations and
requirements emerge.

## Key features

- **Flexible**
  - Our architecture includes various protocols, can be expanded, and meets the technical
    requirements of [**eIDAS 2.0**][eidas] and the **Swiss eID ecosystem**. We take care of
    the complexity and developments around protocols.
- **Interoperable**
  - Uses standardized protocols for credential lifecycles for maximum compatability with
    software from other vendors. See the [supported standards][suppstand] and results of
    [interoperability][interop] testing.
- **Performant**
  - *Procivis One* is scalable and suitable for use cases with millions of users, digital identities
    and credentials.
- **Deployable**
  - *Procivis One* can be installed and operated anywhere: in your data center, at your preferred
    cloud provider or even on IoT devices. The decision is up to you.
- **Privacy by design**
  - Our solution meets the highest data protection requirements such as decentralized data storage,
    data economy and privacy by design.
- **Enterprise ready**
  - *Procivis One* meets all the requirements for productive use by authorities and companies, including
    support and further developments.
- **End-to-end**
  - *Procivis One* covers use cases from issuance to management to verification of digital identities and
    credentials and offers support for all components – from one source.

## Architecture

![Procivis One Core - Architecture](/Procivis_One_Architecture.png)

Use the *Procivis One Core* to build components for your own use case, or use one of the
existing components built on the Core.

### Open source

The following components of *Procivis One* are available with an open source license:

- **Procivis One Core**: handles everything needed to
    issue, hold and verify decentralized digital identity and credentials, and integrates into
    business and IT applications via REST, SDK, or mobile SDK. Use the *Procivis One Core* to build components
    for your own use case, or use one of the existing components built on the Core.
  - [Procivis One Core][core]
- **Procivis One Wallet**: a digital wallet solution that includes the SSI functionality
    of the Core and is available with an open source license. Use the *Procivis One Wallet*
    for a free-standing solution that can be white-labelled, use the *One Core React Native SDK*
    to embed wallet capabilities into an existing app, and use the *One Core React Components* library
    for UI elements for your digital wallet app.
  - [Procivis One Wallet][wallet]
  - [One Core React Native SDK][rncore]
  - [One Core React Native Components][comp]

### Enterprise

The components listed above are available with an Enterprise license, as well as:

- **Procivis One Desk**: a server-based solution that includes the SSI functionality
    of the *Procivis One Core* and adds enterprise functionality such as user and session management, and a
    dashboard for no-code issuance and verification. [Sign up for the trial][trial].
- **Procivis One Verifier**: a mobile verifying solution that includes the SSI
    functionality of the *Procivis One Core* and enables offline verification in both OID4VP and ISO mdoc flows
    over Bluetooth Low Energy (BLE). See the trial version in the iOS and Android app stores.

### Components

The following graphic represents a **component view** of Procivis One. All components
are built from the Procivis One Core and share the same code base.

![Procivis One Components](/Procivis_One_Components.png)

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
