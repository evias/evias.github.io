---
name: Terminal User Interface to run Agentic Intents.
tools: [Go,Cobra,OpenAI,LLM]
image: https://files.evias.be/evias-genesis.png
description: An intent is a pre-configured prompt with arguments
            that is defined using a structured YAML-format.
            The intentd tool features a suite of intents that
            may be run repetitively using your preferred cron system.
---

# intentd: Agentic cronjobs

[![License](https://img.shields.io/github/license/evias/intentd)][license]
[![Website](https://img.shields.io/badge/Website-green.svg)][parent-url]
[![Source code](https://img.shields.io/badge/Source%20code-orange.svg)][code-url]

Use `intentd` to run agentic intents with your provider configuration. 
You may use `intentd` to run any of the pre-configured intents, or
your own intents using the `-I path/to/your/intents` option.

An **intent** is a pre-configured *prompt with arguments* that is defined using
a structured YAML-format to permit rapid fields validation and prompt generation.

The `intentd` tool features a suite of pre-defined *intents* that may be run
repetitively using your preferred cron/PM system.

## What Is Gobots?

Package intentd implements a terminal user interface to run agentic Intents.

An intent is a pre-configured prompt with arguments that is defined using
a structured YAML-format to permit rapid fields validation and prompt generation.

The `intentd` tool features a suite of pre-defined intents that may be run
repetitively using your preferred cron/PM system.

## Usage

```bash
	intentd <intent> [flags]

	Flags:
	-k, --apiKey string         Sets the API Key used for the OpenAI client connection. Required.
	-U, --apiUrl string         Sets the API URL used for the OpenAI client connection (optional). (default "https://ai.chatboxai.app/v1")
	-D, --debug                 Sets whether to enable debug mode/logs or not (optional).
	-h, --help                  help for intentd
	-I, --include stringArray   Specify folders to include for the intents search (optional). (default [intents/])
	-m, --model string          Sets the model that will be used for this conversation (optional). (default "gva/gemini-3.8-flash")
	-o, --output string         Sets an output file to which the response will be appended (optional).
	-Q, --quiet                 Sets whether to enable quiet mode or not (optional).
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
[license]: https://opensource.org/license/mit
[code-url]: https://github.com/evias/intentd
