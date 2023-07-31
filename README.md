# vermont-trustmark
This document is a public description of the State of Vermont's Identity Assurance Levels (IALs) and how the definition of level 1 differs from NIST definitions See [NIST Special Publication 800-63-3 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/). This document's indented audience is the general public and and system engineers.

The Main Difference is this
---------------------------

NIST-800-63-3 defineses Identity Assurance Level 1 (IAL-1) has having "no requirement to link the applicant to a specific real-life identity". Vermont, however, assignes no IAL when creating a my.vermont.gov account. Getting an "IAL-1", in Vermont means something in VT. IAL-1 in VT means that some real-world coreropbiration of a persons identity occured, but it did not meet the stringent requirements of NIST IAL-2.


| LEVEL                  | NIST    |VERMONT|
| -----------            | ------- |------
| "" (Unset)             | -       | This is an untrusted account that has undergone NO identity verification.
| 0 |                    | -       | Administrative reset. IAL may be set to `0` by Vermont.  This may happen to allow Identity verification retry or when the account is suspected to be compromised.|
| 1 | No requirement     | Evidence supports the real-world existence of the claimed identitySome level of identity verification, but does not meet NIST's level 2 definition    |
| 2 | High-level identity assurance    | Same as NIST |
| 3 | Highest-level identity assurance(IAL2)| Same as NIST |

2.2 Identity Assurance Levels

Assurance in a subscriber’s identity is described using one of three IALs:

IAL1: There is no requirement to link the applicant to a specific real-life identity. Any attributes provided in conjunction with the subject’s activities are self-asserted or should be treated as self-asserted (including attributes a CSP asserts to an RP). Self-asserted attributes are neither validated nor verified.

IAL2: Evidence supports the real-world existence of the claimed identity and verifies that the applicant is appropriately associated with this real-world identity. IAL2 introduces the need for either remote or physically-present identity proofing. Attributes could be asserted by CSPs to RPs in support of pseudonymous identity with verified attributes. A CSP that supports IAL2 can support IAL1 transactions if the user consents.

IAL3: Physical presence is required for identity proofing. Identifying attributes must be verified by an authorized and trained CSP representative. As with IAL2, attributes could be asserted by CSPs to RPs in support of pseudonymous identity with verified attributes. A CSP that supports IAL3 can support IAL1 and IAL2 identity attributes if the user consents.


