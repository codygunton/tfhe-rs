# Homomorphic secp256k1 signatures

## Background
In September 2000, the Standards for Efficient Cryptography Group (SECG) published [SEC 2: Recommended Elliptic Curve Domain Parameters](https://www.secg.org/SEC2-Ver-1.0.pdf). The "k" in the name stands for Koblitz, who observed [in 1985 paper](https://link.springer.com/chapter/10.1007/3-540-46766-1_22) that a certain class of elliptic curves admit especially efficient arithmetic via the use of an efficiently computable endomorphism.

The curve secp256k1 plays a central role in  [Bitcoin](https://wiki.bitcoinsv.io/index.php/Secp256k1) and [Ethereum](), where it is used to instantiate the Elliptic Curve Digital Signature Algorithm ([ECDSA](https://en.wikipedia.org/wiki/Elliptic_Curve_Digital_Signature_Algorithm)).

This example shows how to implement ECDSA using secp256k1 in TFHE-rs.