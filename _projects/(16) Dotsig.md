---
name: Dotsig - Digital signatures on the fly
tools: [C++,Botan,ECDSA,PGP,PKCS]
image: https://files.evias.be/evias-genesis.png
description: The **dotsig** software lets you create and verify
            digital signatures using RSA cryptography (PKCS1 v1.5), PGP
            and elliptic-curve cryptography (ECDSA).
---

# Dotsig - Digital signatures on the fly

[![License](https://img.shields.io/github/license/evias/dotsig)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

The **dotsig** software lets you create and verify digital signatures
using RSA cryptography (PKCS1 v1.5), PGP and elliptic-curve cryptography (ECDSA).

This software is released under the [3-Clause BSD License](./LICENSE).

## Releases

The `dotsig` software is currently under active development and frequent changes
to the source code *are to be expected* until the software reaches a stable tag.

The latest release as of May 13th 2024 is: [`v1.1.0-RC.1`][download].

Use `dotsig -v` to find out the version installed on your system.

## Installation

Download the [latest version of `dotsig` here][download] for your system and
install it. Then run one of the commands below to check that your installation
works:

```
dotsig -v
dotsig -h
echo 'Hello, world!' | dotsig
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
[code-url]: https://github.com/evias/dotsig
[download]: https://github.com/evias/dotsig/releases/tag/v1.1.0-RC.1
