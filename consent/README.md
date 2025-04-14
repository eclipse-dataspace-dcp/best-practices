# Discussion on Consent

The specification already mentions parts on consent
in [§ 3.1 Consent](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#consent).

The DCP considers two types of consent

## 1) Consent to Release Claims via Presentation of VCs

When a holder requests a dataset, at first the verifier must specify the required claims to grant access to the data
resource. After this, the consumer must agree to the release of the requested claims. Within the dataspace protocol
stack, this happens in a machine-based fashion through an internal mapping from the policy constraints inside the [DSP
Offer](https://eclipse-dataspace-protocol-base.github.io/DataspaceProtocol/2025-1-RC1/#dfn-offer) to the
corresponding VCs to be released via DCP as described in 
[§ 3.1 Consent](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#consent). Thus, the
claims to be presented may vary by offer. These mappings are dataspace-specific and are outside the scope of the DSP 
or DCP protocol specifications.

## 2) Consent to an Agreement inside DSP

In contrast to the first case, consent to an agreement can either happen in a machine-based fashion or through
manual human approval. In the machine-based case, consent to an agreement is evaluated through an automated policy
evaluation of the DSP request. Alternatively, within the DSP/DCP protocol stack also supports asynchronous
protocol flows to support manual approval through end-user consent.