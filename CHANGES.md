# node-http-signature changelog

## 1.0.0

- First semver release.
- #36: Ensure verifySignature does not leak useful timing information
- #42: Bring the library up to the latest version of the spec (including the 
       request-target changes)
- Support for ECDSA keys and signatures.
- Now uses `sshpk` for key parsing, validation and conversion.
- Fixes for #21, #47, #39 and compatibility with node 0.8

## 0.11.0

- Split up HMAC and Signature verification to avoid vulnerabilities where a
  key intended for use with one can be validated against the other method
  instead.

## 0.10.2

- Updated versions of most dependencies.
- Utility functions exported for PEM => SSH-RSA conversion.
- Improvements to tests and examples.