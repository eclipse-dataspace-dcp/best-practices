# Discussion on Consent

The DCP specification already mentions parts on consent
in [§ 3.1 Consent](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#consent).

The dataspace protocol stack considers two types of consent:

## 1) Consent to Release Claims via Presentation of VCs

When a holder requests a dataset, at first the verifier must specify the required claims to grant access to the data
resource. After this, the consumer must agree to the release of the requested claims. Within the dataspace protocol
stack, this happens in a machine-based fashion through an internal mapping from the policy constraints inside the [DSP
Offer](https://eclipse-dataspace-protocol-base.github.io/DataspaceProtocol/2025-1-RC1/#dfn-offer) to the
corresponding VCs to be released via DCP as described in
[§ 3.1 Consent](https://eclipse-dataspace-dcp.github.io/decentralized-claims-protocol/v1.0-RC2/#consent). Thus, the
claims to be presented may vary by offer. These mappings are dataspace-specific and are outside the scope of the DSP
or DCP protocol specifications.

## 2) Consent to an DSP Contract Negotiation Agreement

In contrast to the first case, consent to a contract negotiation agreement can either take place in a machine-based
fashion or through
manual human approval. To this end, all steps defined in the Contract Negotiation state machine of the DSP
protocol specification (see [DCP Contract Negotiation State Machine](https://eclipse-dataspace-protocol-base.github.
io/DataspaceProtocol/2025-1-RC1/#state-machine)) can be evaluated in a machine-based way by an automated policy
evaluation of the DSP request. However, any of these
steps also support manual approvals instead,
whereby the end-users of the respective organization can approve the agreement instead.

