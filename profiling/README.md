# Best Practices on Profiling the Decentralized Claims Protocol

The [Decentralized Claims Protocol Specification](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol) defines a set of extension points, that need to be populated by profiles. Their main objective is to technically specify the details around Verfiable Credentials. As mentioned in [A.2 Profile Authoring Recommendations](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#profile-authoring-recommendations) of the specification, DCP profiles should define the following aspects to ensure interoperability:

1. VC Data Model
2. Revocation System
3. Proof Stack

Profiles are designated by strings and are used inside the 6.6 `Credential Offer API` and the 6.7 `Issuer Metadata API`. Within this, they define properties of the 6.6.1 `CredentialOfferMessage`, the 6.6.2 `CredentialObject`. Also, within 6.7.1 `Issuer Metadata` a `CredentialObject` is defined.

The two profiles `vc20-bssl/jwt` and `vc11-sl2021/jwt` are recommended by the authors and are therefore defined in the annex of the specification ([A. Profiles of the Decentralized Claims Protocol](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#profiles-of-the-decentralized-claims-protocol)).

Throughout the specificaiton, there is also the definition and the `format` property. While the `format` specifies the used data model and proof stack, the `profile` property additionally covers the specification of the revocation system.