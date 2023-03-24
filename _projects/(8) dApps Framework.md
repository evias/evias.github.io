---
name: dApps Framework
tools: [Blockchain,Healthcare,Smart Contracts,dApps]
image: https://files.evias.be/dhealth-logo.png
description: This framework aims to make it easier to access dHealth Network features and to develop dApps
            with dHealth Network. This software package includes multiple *libraries* and *runtimes* that can be configured separately.
---

[![lerna](https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg)](https://lerna.js.org/)
[![License](https://img.shields.io/badge/License-LGPL%203.0%20only-blue.svg)][license]
[![Discord](https://img.shields.io/badge/chat-on%20discord-green.svg)][discord]

This framework aims to make it easier to access dHealth Network features and to
develop dApps with [dHealth Network][parent-url]. This software package includes
multiple *libraries* and *runtimes* that can be configured separately and that
can be extended and modified freely.

This software lets you connect to [dHealth Public Network](https://dhealth.network) - as well as test networks for dHealth.

## Scopes

This framework implementation features several **application scopes** that are
separately implemented and that can be enabled/disabled by configuration.

Following scopes are defined with their respective description:

| Scope | Documentation | Description |
| --- | --- | --- |
| `common` | `AppModule` | Contains source code that is shared amongst *all* dApps. |
| `discovery` | `DiscoveryModule` | Contains source code for the *discovery* of entities on dHealth Network, e.g. *Transactions*, *Accounts*, *Blocks*, etc. |
| `notifier` | `NotifierModule` | Contains source code to enable maintenance *notifications* that are sent out per email to the team in the case of errors or warnings. |
| `payout` | `PayoutModule` | Contains source code for the *payout of tokens* on dHealth Network. Payouts can be configured to work with any *mosaic* on dHealth Network. |
| `processor` | `ProcessorModule` | Contains source code for the *processor* of entities on dHealth Network. The implementation stores *operations* after reading *transactions*. |
| `statistics` | `StatisticsModule` | Contains source code for the *aggregate of data* related to a dApp. |

**CAUTION**: The above feature scopes *may* be modified in the near- to mid-future,
as we are discovering more use for some of the listed feature scopes.

## Sponsor us

| Platform | Sponsor Link |
| --- | --- |
| Paypal | [https://paypal.me/usingblockchainltd](https://paypal.me/usingblockchainltd) |
| Patreon | [https://patreon.com/usingblockchainltd](https://patreon.com/usingblockchainltd) |
| Github | [https://github.com/sponsors/UsingBlockchain](https://github.com/sponsors/UsingBlockchain) |
| BuyMeACoffee | [https://www.buymeacoffee.com/resoftware](https://www.buymeacoffee.com/resoftware) |
| Bitcoin | `3EVqgUqYFRYbf9RjhyjBgKXcEwAQxhaf6o` |
| Ethereum ERC20 | `0x634061e116F7a043Cf9cE6BE06bF6Efe90EBf9Ef` |


[parent-url]: https://dhealth.com
[license]: https://opensource.org/licenses/LGPL-3.0
[discord]: https://discord.gg/P57WHbmZjk
