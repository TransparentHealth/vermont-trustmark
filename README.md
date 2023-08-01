# vermont-trustmark

Introduction
--------------
This document is a public description of the State of Vermont  classifies identity proofing for individuals. This document's indented audience is the general public and for system engineers implementing systems based on these definitions.

Background
----------
Vermont is leveraging [NIST's Special Publication 800-63-3, "Digital Identity Guidelines"](https://pages.nist.gov/800-63-3/) as a basic approach classifing identity proofing.

Revision 3 of NIST's Digital Identity Guidelines represented a move away from previsous Level of Assurance(LOA) guidance to instead adopt a matrix approach as so :

* AAL - How you log in (Authenticator Assurance)
* IAL - User authenticity(Identity Assurance)
* FAL - Federated Assuance (e.g. connecting to an organization)

The COVID-19 pandemic represented the first time NIST's new IAL defintions, 1, 2, 3 were put to practial use. In healthcare settings, defintions of IAL between 1 and 2 arrose.

Vermont assigns no IAL to new  and untrusted accounts. Some state serviucee may require a trusted account but for a lot of Vermont state services it doesn't matter.

Vermont-trustmark is a profile that sits atop NIST's publication.


The Main Difference is this
---------------------------

NIST-800-63-3 defineses Identity Assurance Level 1 (IAL-1) has having "no requirement to link the applicant to a specific real-life identity". Vermont, however, assignes no IAL when creating a my.vermont.gov account. Getting an "IAL-1", in Vermont means something in VT. IAL-1 in VT means that some real-world coreropbiration of a persons identity occured, but it did not meet the stringent requirements of NIST IAL-2.

Definitions
-----------

See [NIST Special Publication 800-63-3 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/). 




| LEVEL               | DESCRIPTION                                                | NIST      |VERMONT|
| -----------         | ---------------------------------------------------------- | --------- |-------|
| "" (Unset)          | A new My.Vermont.gov account has no identity proofing set. | -         | No ID verification requirement.|
| 0                   | Vewrmont may reset your IAL o `0` for various reasons including when the account is suspected to be compromised. | -       | No ID verification requirement.|
| 1 | No ID verification requirement    | No ID verification requirement     | Somewhat-trusted. n    |
| 2 | High-level identity assurance    | No difference with VT |Same as NIST |
| 3 | DESCRIPTION     |  No difference with VT| Same as NIST |

