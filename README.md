# Awesome-L402

A curated list of awesome things related to L402 ⚡

## Table of Contents

<!-- MarkdownTOC depth=4 -->

- [awesome-l402 ](#awesome-l402-)
  - [Table of Contents](#table-of-contents)
  - [Protocol](#protocol)
  - [Libraries](#libraries)
  - [Projects](#projcets)
  - [Tools](#tools)
  - [Companies](#companies)
  - [Contributing](#contributing)
  - [License](#license)

<!-- /MarkdownTOC -->

<a name="protocol" />

## Protocol

The [L402 protocol](https://docs.lightning.engineering/the-lightning-network/l402), created by [Lightning Labs](https://lightning.engineering), serves as a framework, facilitating service providers in securing their services with a payment gateway.

This setup allows clients to seamlessly transact and gain access to the respective resources. Essentially, it bridges the gap between payment requirements and resource accessibility, streamlining the process for both service providers and their customers.

When a client requests a resource without a valid access token, the server responds with an incomplete token and a Lightning Network invoice for payment. Once the client pays the invoice and obtains a proof of payment, they combine this with the incomplete token to create a valid access token. This complete token, when presented in a subsequent request, is independently verified by the server, confirming the payment and granting access without needing external validation.


- [L402 spec](https://github.com/lightninglabs/L402) - The L402 protocol specification.
- [L420 playground](https://lsat-playground.bucko.vercel.app) - An interactive playground to learn and understand the workings of the protocol.
- [L402 Builder's guide quick start](https://docs.lightning.engineering/the-lightning-network/l402) - LL Builder's guide L402 documentation.
- [L402 Builder's guide spec](https://docs.lightning.engineering/the-lightning-network/l402/protocol-specification) LL Builder's guide protocl spec.
- [Building Paid APIs with Bitcoin](https://www.youtube.com/watch?v=PauSnLTu0BQ) - **Video** Quick overview of the architecture of an L402 by Hannah Rosenberg

The following list will provide you with detailed insights and resources to enhance your understanding of Macaroons and the Lightning Network, the core technologies underpinning the L402 protocol.

- [Lightning network 101](https://docs.lightning.engineering/the-lightning-network/overview) - Learn how the Lightning Network functions.
- [Lightning network spec](https://github.com/lightning/bolts) - BOLT: Basis of Lightning Technology (Lightning Network Specifications)
- [Macaroons: minting and verification](https://github.com/lightninglabs/L402/blob/master/macaroons.md) - Macaroon component in the L402.
- [Macaroons: Cookies with Contextual Caveats for Decentralized Authorization in the Cloud](https://research.google/pubs/macaroons-cookies-with-contextual-caveats-for-decentralized-authorization-in-the-cloud/) - The Research publication introducing Macaroons.
- [Macaroons Overview](https://www.youtube.com/watch?v=CGBZO5n_SUg) - **Video** Talk given at Mozilla by Úlfar Erlingsson

<a name="libraries" />

## Libraries

| Name          | Language      | Overview                                |
|---------------|---------------|-----------------------------------------|
| [aperture/lsat](https://github.com/lightninglabs/aperture/tree/master/lsat) | Go | L402 package used in the Reverse Proxy |
| [l402py](https://github.com/Fewsats/L402py) | python| L402 client and server library for python projects |
| [LangChainBitcoin](LangChainBitcoin) | python | AI tools for giving LangChain agents access to Bitcoin and the ability to traverse L402 APIs |
| [alby-tools](https://github.com/getAlby/js-lightning-tools) | typescript | Collection of helpful building blocks and tools to develop Bitcoin Lightning web apps | 
| [lsat-js](https://github.com/Tierion/lsat-js)  | javascript | A javascript library for working with L402 |


<a name="projects" />

## Projects

- [n8n node](https://github.com/getAlby/n8n-nodes-l402-request) - Node to integrate L402 payments in n8n workflow platform. By Alby.

<a name="tools" />

## Tools

- [Aperture](https://github.com/lightninglabs/aperture) - HTTP 402 reverse proxy that supports proxying requests for gRPC (HTTP/2) and REST (HTTP/1 and HTTP/2) backends using the L402 
- [boltwall](https://github.com/tierion/boltwall) - Bitcoin Lightning paywall and authentication using L402s. Built with LND, Nodejs, and Typescript.
- [Alby](https://getalby.com) - Bitcoin wallet with L402 support


<a name="companies" />

## Companies

- [Lightning Labs](https://lightning.engineering) - Lightning network infrastructure. Created L402 and has been running services supporting (Loop/Pool) the protocol since 2020.
- [Fewsats](https://www.fewsats/com) - *PR incoming.*
- [Sulu](https://www.sulu.sh) - API Monetization with Lightning.
- [Open Agents](https://openagents.com) - An open platform for AI agents, built in public from scratch.
- [Unleashed](https://unleashed.chat) - One button to deploy your own chat.
- [Mash](https://mash.com) - New ways to monetize media.

<a name="contribute" />

## Contribute

Contributions are not only allowed but welcomed!

Feel free to open a PR adding a new entry or section to the repository.

<a name="license" />

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)