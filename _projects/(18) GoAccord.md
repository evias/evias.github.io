---
name: End-to-End Encrypted Messaging with go-accord
tools: [C++,Botan,ECDSA,PGP,PKCS]
image: https://files.evias.be/evias-genesis.png
description: A secure, local, offline, end-to-end encrypted messaging
            for private communication. Built with Go, it features
            BIP32 hierarchical key derivation, ECDH key agreements, and AES-256 encryption and uses a custom YAML-based file
            format for profiles, contacts and messages.
---

# Dotsig - Digital signatures on the fly

[![License](https://img.shields.io/github/license/evias/dotsig)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

A secure, local, offline, end-to-end encrypted messaging for private communication.

Built with Go, it features BIP32 hierarchical key derivation, ECDH key agreements, and AES-256 encryption and uses a custom YAML-based file format for profiles, contacts and messages.

## Features

- **End-to-End Encryption:** Messages encrypted with recipient's public key, decryptable only with their private key
- **Secure Key Management:** BIP32 hierarchical key derivation from BIP39 mnemonics
- **Three-Step Handshakes:** Agree → Accept → Finalize workflow for establishing secure contacts
- **Forward Secrecy:** Unique ephemeral key per message
- **Multi-Machine Support:** Decrypt messages on any machine with the same profile/password
- **Per-Profile Security:** Salted PBKDF2 hashing prevents profile linking
- **Contact Management:** Track handshake identities with public key verification

## Installation

**Requirements:** Go 1.21 or later

```bash
# Clone the repository
git clone https://github.com/resoftware-org/go-accord.git
cd go-accord

# Build
go build -o go-accord

# Verify
./go-accord --help
```

## Sponsor us

| Platform | Sponsor Link |
| --- | --- |
| Paypal | [https://paypal.me/usingblockchainltd](https://paypal.me/usingblockchainltd) |
| Patreon | [https://patreon.com/usingblockchainltd](https://patreon.com/usingblockchainltd) |
| Github | [https://github.com/sponsors/UsingBlockchain](https://github.com/sponsors/UsingBlockchain) |
| BuyMeACoffee | [https://www.buymeacoffee.com/resoftware](https://www.buymeacoffee.com/resoftware) |
| Bitcoin | `3EVqgUqYFRYbf9RjhyjBgKXcEwAQxhaf6o` |
| Ethereum ERC20 | `0x634061e116F7a043Cf9cE6BE06bF6Efe90EBf9Ef` |

[parent-url]: https://resoftware.es/get-a-free-quote/
[license]: https://opensource.org/license/bsd-3-clause
[code-url]: https://github.com/resoftware-org/go-accord
