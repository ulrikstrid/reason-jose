0.6.0
--------------
- JWT/JWS/JWK: Add support for ES256 and ES512 signing via the updated mirage-crypto and x509 (by @ulrikstrid)
- JWT: [BREAKING] JWT will not validate `exp` by default anymore (by @ulrikstrid)

0.5.1
--------------
- JWA: Add Unsupported option and stop raising when encountering unknown `kty` (by @ulrikstrid)

0.5.0
--------------
- JWS: compare computed HMAC signatures in constant-time (by @anmonteiro)
- Adapt to Mirage-crypto 0.8.1, drops support for OCaml < 4.8.0 (breaking) (by @anmonteiro)

0.4.0
--------------
- RFC7638: Implement thumbprints (by @undu)
- Make kid optional in the header and jwk

0.3.1
--------------
- Add result compatability package (by @anmonteiro)
- Add `kid` to JWK representation to keep it when parsing JSON input
- Fix upper constraint on mirage-crypto

0.3.0
--------------
- Change the JWT representation to be based on a GADT, this allows us to use a private JWT for anything where a public JWT is enough.
- Add JWE encryption and decryption

0.2.0
--------------
- Change from nocrypto to mirage

0.1.0
--------------
- Initial release
