---
name: Smaili the Micro Rover
tools: [C++,Arduino,IDE]
image: https://files.evias.be/evias-genesis.png
description: A tiny *smiling* rover that speaks JSON. This project
            contains the firmware source code (C++) for a ESP32 DEVKIT V1
            board that can be flashed using Arduino IDE.
---

# Smaili the Micro Rover

[![License](https://img.shields.io/github/license/evias/dotsig)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

A tiny *smiling* (:smiley:) rover that speaks JSON!

This project contains the firmware source code (C++) for a ESP32 DEVKIT V1 board which is wired together with listed components. Note that for practicability, the ESP32 board is plugged on a `10:30` prototyping breadboard and attached to the bottom plate of the rover platform.

## Usage

Example commands that you may send over Serial port, e.g. using Serial Monitor plugin for VSCode and/or Arduino IDE:

### Status command
```json
{"command":"status"}
```

### Start/Stop commands

```json
{"command":"start","options":{"side":"right","duration":3000}}
{"command":"stop","options":{"side":"right"}}
```

### Turn command

```json
{"command":"turn","options":{"angle":10}}
{"command":"turn","options":{"angle":140}}
```

### Scan command

```json
{"command":"scan","options":{"count":5,"interval":500}}
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
[code-url]: https://github.com/evias/smaili-the-micro-rover
