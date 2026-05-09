# ThinMemory Revocation List Repository

This repository distributes signed ThinMemory license revocation list (TMRL) artifacts.

## Trust Model

Artifacts in this repository are signed with the ThinMemory commercial Ed25519 signing key. Manager binaries verify the signature using an embedded public key before trusting any artifact contents. TLS is not load-bearing for trust — the signature is. This repository may be fetched over plain HTTP without compromising security.

## Artifact Location

The current revocation list is always at: revocation/current.tmrl

## For ThinMemory Users

Your ThinMemory installation fetches this list automatically. No user action required.

## For Researchers

The TMRL binary format will be documented in the ThinMemory public specification when the revocation infrastructure sub-phase is complete.
