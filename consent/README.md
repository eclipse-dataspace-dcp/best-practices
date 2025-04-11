# Discussion on Consent

The specification already mentions parts on consent in [§ 3.1 Consent](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#consent). 

The DCP considers two types of consent
## 1) Consent to Release Claims (via Presentation of VCs)
When a consumer requests a dataset, at first the provider must specify the required claims to grant access to the data resource. After this, the consumer must agree to the release of the requested claims. Within the dataspace protocol stack, this happens in a machine-based fashion through an internal mapping between the DCP policy constraints and the corresponding Verifiable Credentials to be released via DCP. These mappings are always dataspace-specific and outside the scope of the protocol specifications.

## 2) Consent to an Agreement
In contrast to the first case, consent to an agreement can either also happen in a machine-based fashion or through manual human approval. In the machine-based case, consent to an agreement is evaluated through an automated policy evaluation of the DSP request. Alternatively, the DCP also supports asynchronous protocol flows to support manual approval through end-user consent.