## Overview

The original [JSON Object Signing and Encryption (JOSE) working group](https://datatracker.ietf.org/doc/charter-ietf-jose/02/) standardized JSON-based representations for: Integrity-protected objects (JSON Web Signatures/JWS, RFC 7515), Encrypted objects (JSON Web Encryption/JWE, [RFC7516](https://datatracker.ietf.org/doc/rfc7516/)), Key representations (JSON Web Key/JWK, [RFC7517](https://datatracker.ietf.org/doc/rfc7517/)), Algorithm definitions (JSON Web Algorithms/JWA, [RFC7518](https://datatracker.ietf.org/doc/rfc7518/)), and Test vectors for the above (Examples of Protecting Content Using JSON Object Signing and Encryption, [RFC7520](https://datatracker.ietf.org/doc/rfc7520/)).

These were used to define the JSON Web Token (JWT) ([RFC7519](https://datatracker.ietf.org/doc/rfc7519/)), which in turn, has seen widespread deployment in areas as diverse as [digital identity](https://openid.net/connect/) and [secure telephony](https://www.ietf.org/blog/stir-action/).

As adoption of these standards to express and communicate sensitive data has grown, so too has an increasing societal focus on privacy. User consent, minimal disclosure, and unlinkability are common privacy themes in identity solutions.

A multi-decade research activity for a sizeable academic and applied cryptography community has focused on these privacy and knowledge mechanisms (often referred to as anonymous credentials). Certain cryptographic techniques developed in this space involve pairing-friendly curves and zero-knowledge proofs (ZKPs) (to name just a few). Some of the benefits of ZKP algorithms include unlinkability, selective disclosure, and the ability to use predicate proofs.

The current container formats defined by JOSE and JWT are not able to represent data using ZKP algorithms. Among the reasons are that most require an additional transform or finalize step, many are designed to operate on sets and not single messages, and the interface to ZKP algorithms has more inputs than conventional signing algorithms. The reconstituted JOSE working group will address these new needs, while reusing aspects of JOSE and JWT, where applicable.

The JOSE working group will also maintain the JOSE standard and facilitate discussion of clarifications, improvements, and extensions to JWS, JWE, JWA, and JWK. The WG will evaluate, and potentially adopt, proposed standard documents dealing with algorithms that would fit the criteria of being IETF consensus algorithms. Potential candidates would include those algorithms that have been evaluated by the CFRG and algorithms which have gone through a public review and evaluation process such as was done for the NIST SHA-3 algorithms. Potential candidates would not include national-standards-based algorithms that have not gone through a similar public review process. The WG may also publish informational and BCP documents describing the proper use of these algorithms in JOSE.

An informal goal of the working group is close coordination with the rechartered W3C Verifiable Credentials WG, which has taken a dependency on this work for the second version of its Verifiable Credentials specification. The working group will also coordinate with the [Selective Disclosure JWT](https://datatracker.ietf.org/doc/draft-ietf-oauth-selective-disclosure-jwt/) work in the [OAuth working group](https://datatracker.ietf.org/wg/oauth/about/), the Privacy Pass working group, the [CBOR working group](https://datatracker.ietf.org/wg/cbor/about/), the [COSE working group](https://datatracker.ietf.org/wg/cose/about/), and the [CFRG](https://datatracker.ietf.org/rg/cfrg/about/).

# Contributing

Learn about the [IETF process](https://www.ietf.org/process/process/).

[Reporting protocol vulnerabilities to the IETF](https://www.ietf.org/process/rfcs/vulnerabilities/).

## Mailing List

- [Subscribe](https://www.ietf.org/mailman/listinfo/jose)
- [View the Archive](https://mailarchive.ietf.org/arch/browse/jose/)
