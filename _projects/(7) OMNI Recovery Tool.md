---
name: OMNI Recovery Tool
tools: [PHP7,Laravel,Bitcoin,USDT,Recovery]
image: https://files.evias.be/yourdlt-logo.png
description: The evias/omni-recovery-tool Package aims to be an easy to use command line interface and
            API utility Software built around Bitcoin, Colored Coins (OMNI / Tether USDT), NEM and dHealth Network blockchain features.
---

# OMNI Recovery Tool

[![License](https://img.shields.io/badge/License-LGPL%203.0%20only-blue.svg)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

The evias/omni-recovery-tool Package aims to be an easy to use command line
interface and API utility Software built around Bitcoin, Colored Coins
(OMNI / Tether USDT), NEM and dHealth Network blockchain features.

## Usage Examples

```bash
# Get list of available commands
$ php application list

# Get Simple HD Address from BIP32 Extended Public Key
$ php application wallet:hd-from-xpub --xpub="xpub123456"

# Get BIP44 Addresses, Public Keys and Private Keys
$ php application wallet:derive --mnemonic="abandon abandon abandon" --path="m/44'/0'/0'/0"

# Parse a OP_RETURN colored coin hexadecimal payload (Omnilayer or any other OP_RETURN content)
$ php application script:op-return --asm="OP_RETURN 6f6d6e69000000000000001f000000002faf0800 OP_EQUAL"
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

[parent-url]: https://ubc.digital
[license]: https://opensource.org/licenses/LGPL-3.0
[code-url]: https://github.com/evias/omni-recovery-tool
