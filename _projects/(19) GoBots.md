---
name: Gobots protocol for connected edge devices.
tools: [Go,Cobra,TCP,BLE,Serial]
image: https://files.evias.be/evias-genesis.png
description: A comprehensive communication protocol for connected
            edge devices. gobots is a software package that introduces
            the concept of botfiles which describe commands, tasks and
            workflows executed by robots, or any type of edge devices.
---

# Gobots - Connected edge devices

[![License](https://img.shields.io/github/license/evias/gobots)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

`gobots` is a software package that introduces the concept of `botfiles`
which describe commands, tasks and workflows executed by *robots*,
or any type of edge devices.

In short: **Sick of reverse-engineering communication protocols for your devices?**
Now is the time to switch to `gobots`, probability has it that at least someone
on the Internet has already described/mapped your edge device into a `botfile`.

## What Is Gobots?

Package gobots defines structures and interfaces to connect and communicate
with robot devices and/or any connected edge devices.

The `gobots` software introduces **botfile**s and the **Wire protocol** to
facilitate inter-devices communication over network or serial connections.

- The `robot.Robot` structure provides a connection wrapper and communication
channel for connected edge devices. This implementation is agnostic to the
actual edge devices' hardware and installed firmware.
- A `cmd` package is provided which serves as a first draft interface for
connection and communication with supported edge devices through YAML driver
files and the Wire messaging format.

## Usage

A terminal user interface is provided with an interactive console to connect
directly with edge devices and execute commands:

```bash
# Open an interactive console to a device using a driver file
$ gobots console drivers/ELEGOO/smartcar-v4.yaml

# Open an interactive console to a device using a custom host and port
$ gobots console 192.168.4.1:100 -d drivers/ELEGOO/smartcar-v4.yaml

# Execute commands with parameters from the console directly
bot> exec move --speed 10 --direction forward
bot> exec stop
```

Connect and execute commands directly with `gobots exec`:

```bash
$ gobots exec move --speed 10 --direction forward -d drivers/ELEGOO/smartcar-v4.yaml
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
[code-url]: https://github.com/evias/gobots
