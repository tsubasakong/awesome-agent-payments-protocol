# Awesome Agent Payments Protocol [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🚀 Curated resources for the **agentic commerce** protocol landscape — **UCP**, **AP2**, **A2A**, **x402**, **ACP**, **MPP**, trust rails, and interop standards.

**PRs welcome!** Found something amazing? [Open a PR](../../pulls) or [suggest a resource](../../issues/new?template=add_resource.yml) 🎯

*Last updated: 2026-03-23*

---

## 📋 Contents

- [Official Documentation](#-official-documentation)
  - [UCP (Universal Commerce Protocol)](#ucp-universal-commerce-protocol)
  - [AP2 (Agent Payments Protocol)](#ap2-agent-payments-protocol)
  - [A2A (Agent-to-Agent Protocol)](#a2a-agent-to-agent-protocol)
  - [x402 (Machine Payments over HTTP 402)](#x402-machine-payments-over-http-402)
  - [ACP (Agentic Commerce Protocol)](#acp-agentic-commerce-protocol)
  - [MPP (Machine Payments Protocol)](#mpp-machine-payments-protocol)
  - [Network Trust Rails for Agents](#network-trust-rails-for-agents)
  - [Identity / Interop](#identity--interop)
- [Specifications & Whitepapers](#-specifications--whitepapers)
- [Developer Tools & Starters](#-developer-tools--starters)
- [Ecosystem & Partners](#-ecosystem--partners)
- [News & Analysis](#-news--analysis)
- [Videos & Tutorials](#-videos--tutorials)
- [Community](#-community)

---

## 📚 Official Documentation

### UCP (Universal Commerce Protocol)

- [UCP Official Site](https://ucp.dev/) — Protocol overview, spec, tutorials, and guides
- [Google Developers: UCP Guide](https://developers.google.com/merchant/ucp) — Integration guide for merchants
- [UCP GitHub Repository](https://github.com/Universal-Commerce-Protocol/ucp) — Specification and documentation
- [Under the Hood: UCP (Google Developers Blog)](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/) — Technical deep dive (Jan 2026)
- [UCP Launch Announcement (Google Blog)](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/) — NRF 2026 announcement
- [Shopify Engineering: Building UCP](https://shopify.engineering/ucp) — Architecture and layered protocol design
- [UCP and AP2](https://ucp.dev/) — How UCP integrates with AP2 for secure payments (see "UCP and AP2" section on site)
- [UCP Updates (Mar 2026)](https://blog.google/products-and-platforms/products/shopping/ucp-updates/) — Multi-item carts, catalog queries, identity linking

### AP2 (Agent Payments Protocol)

- [AP2 Protocol Documentation](https://ap2-protocol.org/) — Overview, mandate types, A2A/MCP relationships, and integrations
- [AP2 Specification](https://ap2-protocol.org/specification/)
- [AP2 GitHub Repository](https://github.com/google-agentic-commerce/AP2) — Spec, Python & Android samples
- [Google Cloud AP2 Announcement](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol)
- [AP2 Roadmap](https://ap2-protocol.org/) — See roadmap section on official site
- [AP2 Partners](https://ap2-protocol.org/) — See partners section on official site
- [AP2 and UCP](https://ap2-protocol.org/) — How AP2 provides the payment mandate layer for UCP

### A2A (Agent-to-Agent Protocol)

- [A2A Protocol Site](https://a2a-protocol.org/latest/) — Official documentation and specification
- [Announcing Version 1.0](https://a2a-protocol.org/latest/announcing-1.0/) — v1.0 release with enterprise features, signed agent cards, multi-tenancy
- [What's New in v1.0](https://a2a-protocol.org/latest/whats-new-v1/) — Migration guide from v0.3 to v1.0
- [A2A Specification](https://a2a-protocol.org/latest/specification/) — Full protocol spec (JSON-RPC 2.0 over HTTP, gRPC, SSE)
- [A2A GitHub Repository](https://github.com/a2aproject/A2A)
- [A2A Samples](https://github.com/a2aproject/a2a-samples)
- [A2A x402 Extension](https://github.com/google-agentic-commerce/a2a-x402) — Payment extension for A2A using x402
- [A2A Project (Linux Foundation)](https://www.linuxfoundation.org/press/linux-foundation-launches-the-agent2agent-protocol-project-to-enable-secure-intelligent-communication-between-ai-agents)
- [ADK A2A Guides](https://google.github.io/adk-docs/a2a/)

#### A2A SDKs

| Language | Repository | Status |
|----------|-----------|--------|
| Python | [a2aproject/a2a-python](https://github.com/a2aproject/a2a-python) | Stable (v0.3); v1.0 alpha in `1.0-dev` branch |
| JavaScript | [a2aproject/a2a-js](https://github.com/a2aproject/a2a-js) | Stable |
| Go | [a2aproject/a2a-go](https://github.com/a2aproject/a2a-go) | Stable |
| Java | [a2aproject/a2a-java](https://github.com/a2aproject/a2a-java) | Stable |
| .NET | [a2aproject/a2a-dotnet](https://github.com/a2aproject/a2a-dotnet) | Preview ([Microsoft Foundry blog](https://devblogs.microsoft.com/foundry/building-ai-agents-a2a-dotnet-sdk/)) |

### x402 (Machine Payments over HTTP 402)

- [x402.org](https://www.x402.org/) — Protocol homepage
- [x402 Developer Docs](https://docs.x402.org/) — Core concepts, quickstarts, guides (docs.x402.org / Mintlify)
- [x402 GitHub Repository](https://github.com/coinbase/x402) — Spec, SDKs (TypeScript, Python, Go), and examples
- [x402 Whitepaper (PDF)](https://www.x402.org/x402-whitepaper.pdf)
- [Quickstart for Buyers](https://docs.cdp.coinbase.com/x402/quickstart-for-buyers)
- [Quickstart for Sellers](https://docs.cdp.coinbase.com/x402/quickstart-for-sellers)
- [MCP Server with x402](https://docs.cdp.coinbase.com/x402/mcp-server) — Guide for monetizing MCP tools with x402
- [Migration Guide (v1 → v2)](https://docs.cdp.coinbase.com/x402/migration-guide) — Standardized CAIP identifiers, modular SDK, new headers
- [x402 V2 Launch Post](https://www.x402.org/writing/x402-v2-launch)
- [Cloudflare Agents SDK: x402](https://developers.cloudflare.com/agents/x402/) — Built-in x402 support in Cloudflare Workers
- [Cloudflare Blog: x402 Foundation](https://blog.cloudflare.com/x402/) — x402 Foundation announcement with Coinbase

### ACP (Agentic Commerce Protocol)

> **Note:** The ACP spec is currently in **beta** and uses date-based version snapshots (2025-09-29, 2025-12-12, 2026-01-16, 2026-01-30).

- [ACP Spec Site](https://agenticcommerce.dev/) — Protocol overview and interactive demo
- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started)
- [ACP: Key Concepts](https://developers.openai.com/commerce/) — Protocol page on OpenAI Developers
- [ACP: Product Feeds](https://developers.openai.com/commerce/) — Product feed spec for merchant integration
- [ACP: Agentic Checkout Spec](https://developers.openai.com/commerce/) — Checkout flow and endpoints
- [ACP: Delegated Payment Spec](https://developers.openai.com/commerce/) — Shared Payment Token and PSP integration
- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) — Spec, RFCs, examples, changelog
- [OpenAI: Buy it in ChatGPT](https://openai.com/index/buy-it-in-chatgpt/) — Instant Checkout launch post

#### Stripe ACP / Agentic Commerce Resources

- [Stripe: Integrate the ACP](https://docs.stripe.com/agentic-commerce/protocol) — RESTful or MCP server implementation guide
- [Stripe: Shared Payment Token](https://docs.stripe.com/agentic-commerce/) — Payment primitive for agentic flows
- [Stripe Blog: Developing an Open Standard for Agentic Commerce](https://stripe.com/blog/developing-an-open-standard-for-agentic-commerce)

### MPP (Machine Payments Protocol)

- [MPP Official Site](https://mpp.dev/overview) — Protocol overview, SDKs, and quickstart
- [Stripe: Machine Payments with MPP](https://docs.stripe.com/payments/machine/mpp) — Implementation docs (crypto + fiat via PaymentIntents)
- [Stripe Blog: Introducing MPP](https://stripe.com/blog/machine-payments-protocol) — Launch post (Mar 2026)
- [Cloudflare Agents Docs: MPP](https://developers.cloudflare.com/agents/agentic-payments/mpp/) — MPP integration in Cloudflare Workers
- [IETF Draft: Payment HTTP Authentication Scheme](https://mpp.dev/overview) — See spec link on mpp.dev

> **MPP and x402:** MPP is backwards-compatible with x402. The core x402 exact-payment flows map directly onto MPP's `charge` intent, so MPP clients can consume existing x402 services without modification. MPP additionally supports `session` (streaming/pay-as-you-go) payments, recurring payments, and microtransactions across stablecoins, cards, and bank transfers.

### Network Trust Rails for Agents

#### Visa Trusted Agent Protocol

- [Press Release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare Press Note](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)

#### Mastercard Agent Pay

- [Press Release (Sep 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/september/mastercard-unveils-new-tools-and-collaborations-to-power-smarter%2C-safer-agentic-commerce.html)
- [Initial Announcement (Apr 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai.html)

### Identity / Interop

- [Model Context Protocol (MCP) — Spec & Docs](https://modelcontextprotocol.io/) — Standard for AI agent tool interoperability
- [MCP Specification (GitHub)](https://github.com/modelcontextprotocol/specification) — Protocol spec repository
- [MCP Registry (Preview)](https://github.com/mcp) — GitHub MCP Registry for discovering MCP servers
- [Web Bot Auth — Architecture Draft (IETF)](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-architecture) — Agent identity via HTTP Message Signatures
- [Web Bot Auth — Directory Draft (IETF)](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-directory) — Directory for verified bot identities
- [Web Bot Auth (Cloudflare Developer Docs)](https://developers.cloudflare.com/bots/reference/bot-verification/web-bot-auth/)

---

## 📄 Specifications & Whitepapers

### x402 Protocol

- [x402 Whitepaper (PDF)](https://www.x402.org/x402-whitepaper.pdf)
- [x402 Spec & Reference (GitHub)](https://github.com/coinbase/x402)

### A2A & AP2

- [A2A v1.0 Specification](https://a2a-protocol.org/latest/specification/)
- [AP2 Specification](https://ap2-protocol.org/specification/)
- [UCP Specification](https://ucp.dev/) — Full spec at ucp.dev

### ACP

- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) — Versioned snapshots (2025-09-29 through 2026-01-30)

### MPP

- [MPP Overview & Spec](https://mpp.dev/overview) — Protocol specification and payment flow documentation
- [IETF Payment HTTP Authentication Scheme](https://mpp.dev/overview) — See spec link on mpp.dev

### Web Bot Auth / Agent Identity

- [IETF Draft — Web Bot Auth Architecture](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-architecture)
- [IETF Draft — Web Bot Auth Directory](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-directory)

### Research Papers

- "Towards Multi-Agent Economies: A2A + x402 Micropayments" — Proposes ledger-anchored identities with x402 for A2A micropayments

---

## 🛠 Developer Tools & Starters

### UCP Implementation

- [UCP GitHub Repository](https://github.com/Universal-Commerce-Protocol/ucp) — Spec, SDKs (Python, JavaScript), and reference implementations
- [UCP Python Sample](https://github.com/Universal-Commerce-Protocol/ucp) — See `samples/` in the repo
- [Google Merchant UCP Integration Guide](https://developers.google.com/merchant/ucp)

### AP2 Implementation

- [AP2 Python & Android Samples](https://github.com/google-agentic-commerce/AP2)

### x402 Implementation

#### Quickstarts

- [Quickstart for Sellers](https://docs.cdp.coinbase.com/x402/quickstart-for-sellers)
- [Quickstart for Buyers](https://docs.cdp.coinbase.com/x402/quickstart-for-buyers)
- [MCP Server with x402](https://docs.cdp.coinbase.com/x402/mcp-server)
- [QuickNode — Using x402 for Paywalls](https://www.quicknode.com/guides/infrastructure/how-to-use-x402-payment-required)
- [Crossmint x402 Starter](https://github.com/Crossmint/crossmint-402-starter)

#### SDKs & Libraries

- [x402 Monorepo (GitHub)](https://github.com/coinbase/x402) — `@x402/core`, `@x402/evm`, `@x402/svm`, `@x402/axios`, `@x402/fetch`, `@x402/express`, `@x402/hono`, `@x402/next`, `@x402/paywall`
- [x402 Rust crates + Facilitator](https://github.com/x402-rs/x402-rs)

### ACP Implementation

- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started/)
- [ACP Spec & Examples (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol)
- [Stripe: Integrate the ACP](https://docs.stripe.com/agentic-commerce/protocol)

### MPP Implementation

- [MPP SDKs](https://mpp.dev/overview) — Official TypeScript SDK (`mppx`) with middleware for Hono, Express, Next.js, Elysia
- [Stripe: Machine Payments with MPP](https://docs.stripe.com/payments/machine/mpp) — Implementation with PaymentIntents

### A2A Implementation

- [A2A Samples Repository](https://github.com/a2aproject/a2a-samples) — Hello-world, multi-agent, and framework-specific examples
- [A2A Inspector](https://github.com/a2aproject/a2a-inspector) — Validate your A2A agent

### Agent Frameworks

#### Cloudflare Agents SDK

- [Agents SDK Overview](https://developers.cloudflare.com/agents/)
- [x402 in Agents SDK](https://developers.cloudflare.com/agents/x402/) — Built-in x402 support
- [MPP in Agents SDK](https://developers.cloudflare.com/agents/agentic-payments/mpp/) — Built-in MPP support
- [Cloudflare Blog: x402 Foundation](https://blog.cloudflare.com/x402/)

#### MCP Integration

- [OpenAI Agents SDK — MCP](https://openai.github.io/openai-agents-python/mcp/)
- [Stripe MCP Server](https://docs.stripe.com/) — Stripe's MCP tools for agentic commerce

---

## 🌐 Ecosystem & Partners

### UCP

Co-developed by **Google** and **Shopify**. Endorsed by 20+ partners including Etsy, Wayfair, Target, Walmart, Adyen, American Express, Best Buy, Flipkart, Macy's Inc., Mastercard, Stripe, The Home Depot, Visa, and Zalando. ([Source: Google Blog, Jan 2026](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/))

### AP2

Officially reported supporters include Shopify, Etsy, Salesforce, Mastercard, PayPal, American Express, Adyen, Worldpay, and 60+ partners total. ([Source: AP2 Protocol site](https://ap2-protocol.org/))

### x402 Foundation

**Cloudflare + Coinbase** coordinating adoption of x402. The Agents SDK and MCP servers support x402 out of the box. x402 v2 adds modular payment scheme support for EVM and Solana networks.

### ACP

**OpenAI + Stripe** co-developed ACP. Currently live with Instant Checkout in ChatGPT (US). Initial merchant partners include Etsy (live) and Shopify merchants (rolling out). ACP is open to any PSP — Stripe is the first with its Shared Payment Token. The spec is in **beta** with active iteration. ([Source: OpenAI](https://openai.com/index/buy-it-in-chatgpt/))

### MPP / Tempo

**Stripe + Tempo Labs (Paradigm)** co-authored MPP. Design partners include Anthropic, DoorDash, Mastercard, Nubank, OpenAI, Ramp, Revolut, Shopify, Standard Chartered, and Visa. Cloudflare supports MPP in its Agents SDK. ([Source: Stripe Blog, Mar 2026](https://stripe.com/blog/machine-payments-protocol))

### Agent Trust Rails

**Visa's Trusted Agent Protocol** and **Mastercard's Agent Pay** both leverage **Web Bot Auth** for cryptographically signed agent identity during browse and payment flows.

### Payments Networks

- **Visa** — Trusted Agent Protocol
- **Mastercard** — Agent Pay; acquired BVNK for stablecoin infrastructure
- **PayPal** — AP2 support; upcoming UCP payment method
- **American Express** — AP2 partner, UCP endorser
- **Adyen** — AP2 integration, UCP endorser
- **Worldpay** — AP2 support
- **Stripe** — ACP co-creator, MPP co-author, UCP endorser

### AI / Agent Platforms

- **Google Cloud** — AP2 creator, UCP co-developer
- **OpenAI** — ACP co-creator (with Stripe)
- **Anthropic** — MPP design partner
- **Shopify** — UCP co-developer, AP2 & ACP partner

### Crypto & Web3

- **Coinbase** — x402 creator, AP2 partner
- **Tempo Labs** — MPP co-author (Paradigm-backed, payments-optimized L1)
- **Radius Network** — x402-compatible stablecoin L1 for agentic micropayments

---

## 📰 News & Analysis

### Major Launches & Milestones

#### UCP Launch (January 2026)

- [Google Blog: New tech and tools for retailers (NRF 2026)](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/)
- [Google Developers Blog: Under the Hood of UCP](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/)
- [UCP Updates: Multi-item carts, catalog, identity linking (Mar 2026)](https://blog.google/products-and-platforms/products/shopping/ucp-updates/)

#### A2A v1.0 (2026)

- [A2A: Announcing Version 1.0](https://a2a-protocol.org/latest/announcing-1.0/) — Enterprise features, signed agent cards, multi-tenancy

#### MPP Launch (March 2026)

- [Stripe Blog: Introducing MPP](https://stripe.com/blog/machine-payments-protocol)
- [Cloudflare Agents Docs: MPP](https://developers.cloudflare.com/agents/agentic-payments/mpp/)

#### x402 V2 (Late 2025 – Early 2026)

- [x402 V2 Launch Post](https://www.x402.org/writing/x402-v2-launch)
- [Cloudflare Agents SDK v0.4.0: x402 v2 migration](https://developers.cloudflare.com/changelog/post/2026-02-09-agents-sdk-v040/)

#### AP2 Launch (September 2025)

- [TechCrunch: Google launches new protocol for agent-driven purchases](https://techcrunch.com/2025/09/16/google-launches-new-protocol-for-agent-driven-purchases/)
- [Axios: Google's AP2 aims to boost trust in agent shopping](https://www.axios.com/2025/09/16/google-ai-agents-ecommerce-online-shopping)
- [Digital Commerce 360: AP2 gains support from Shopify, Etsy](https://www.digitalcommerce360.com/2025/09/19/google-ai-payments-protocol-ap2/)

#### OpenAI Instant Checkout & ACP (September 2025)

- [Reuters: OpenAI partners with Etsy, Shopify for ChatGPT checkout](https://www.reuters.com/world/americas/openai-partners-with-etsy-shopify-chatgpt-checkout-2025-09-29/)
- [AP News: OpenAI Instant Checkout coverage](https://apnews.com/article/openai-chatgpt-shopping-etsy-shopify)
- [Stripe Blog: Developing an Open Standard for Agentic Commerce](https://stripe.com/blog/developing-an-open-standard-for-agentic-commerce)

#### x402 Foundation (2025)

- [Cloudflare Blog: x402 Foundation announcement](https://blog.cloudflare.com/x402/)

#### Network Trust Rails (2025)

- [Visa: Trusted Agent Protocol press release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare: Collaboration with payments companies](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)

### Industry Analysis

- [Constellation Research: Google's AP2 fleshes out AI agent commerce](https://www.constellationr.com/blog-news/insights/googles-agent-payments-protocol-fleshes-out-ai-agent-commerce)
- [Finextra Deep Dive: Google's AP2 explained](https://www.finextra.com/blogposting/29408/deep-dive-googles-ap2-explained---the-rulebook-for-agent-led-payments)
- [PYMNTS: Google unveils payment protocol for AI-driven commerce](https://www.pymnts.com/artificial-intelligence-2/2025/google-unveils-a-payment-protocol-for-ai-driven-commerce/)
- [Digital Commerce 360: OpenAI expands agentic commerce push (Feb 2026)](https://www.digitalcommerce360.com/2026/02/16/openai-expands-agentic-commerce-push/)

### Security & Standards

- [Cloud Security Alliance: Secure Use of AP2](https://cloudsecurityalliance.org/blog/2025/10/06/secure-use-of-the-agent-payments-protocol-ap2-a-framework-for-trustworthy-ai-driven-transactions)
- [PayPal Dev Blog: AP2 mandates as W3C VCs](https://developer.paypal.com/community/blog/PayPal-Agent-Payments-Protocol/)

---

## 🎥 Videos & Tutorials

### AP2

- [Intro to Google Agent Payments Protocol (AP2)](https://www.youtube.com/watch?v=yLTp3ic2j5c) — Beginner-friendly introduction
- [AP2 Overview & Ecosystem Breakdown](https://www.youtube.com/watch?v=m03UOWQIiJo) — Comprehensive ecosystem analysis
- [Technical Review: AP2 Code Walkthrough (Kotlin)](https://www.youtube.com/watch?v=5-B86E6w2t4) — Code implementation review
- [AP2 Core Concept: Signed Authorization & Accountability](https://www.youtube.com/shorts/OUITfQDEn3k) — Short-form explanation
- [After MCP & A2A, Meet AP2](https://www.youtube.com/watch?v=vxRe33XUMQY) — Protocol evolution overview

### x402

- [x402 Deep Dive & Demos](https://www.youtube.com/watch?v=pL5LxhZ8iCY) — Technical walkthrough
- [x402 Short Explainer](https://www.youtube.com/shorts/tgpVtCdu3tU) — Quick overview

### ACP

- [OpenAI: Buy it in ChatGPT (ACP)](https://openai.com/index/buy-it-in-chatgpt/) — Official product demo

### A2A

- [A2A Protocol Short Course (DeepLearning.AI)](https://github.com/a2aproject/A2A) — Built with Google Cloud and IBM Research (see repo for link)

---

## 💬 Community

### Discussion & Support

- [Google Developers Community: AP2 Introduction](https://discuss.google.dev/t/new-agent-payments-protocol-ap2-an-open-and-secure-standard-for-agentic-payments/265614)
- [x402 Community FAQ](https://docs.cdp.coinbase.com/x402/support/faq) — FAQ & Discord links
- [A2A GitHub Discussions](https://github.com/a2aproject/A2A/discussions)

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **📝 Add a resource:** [Use our template](../../issues/new?template=add_resource.yml)
2. **🔧 Improve the list:** Submit a [pull request](../../pulls)
3. **🐛 Report issues:** [Open an issue](../../issues/new)
4. **⭐ Star the repo** to show your support!

Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting.

---

## 📊 About These Protocols

**UCP (Universal Commerce Protocol)** is an open standard co-developed by Google and Shopify for agentic commerce across the full shopping journey — discovery, checkout, identity linking, and order management. UCP is transport-agnostic (REST, MCP, A2A) and compatible with AP2 for secure payment mandates. Launched January 2026 at NRF.

**AP2 (Agent Payments Protocol)** is Google's open protocol for agent-driven payments with verifiable authorization (mandates) and accountability. Its current core focus is card-based payments with mandate-driven authorization. AP2 serves as the payment layer within UCP.

**A2A (Agent-to-Agent Protocol)** is an open standard under the Linux Foundation for agent interoperability — discovery, communication, and task delegation across agent frameworks and vendors. The v1.0 release (2026) added enterprise features including signed agent cards, multi-tenancy, and version negotiation. The TSC includes AWS, Cisco, Google, IBM Research, Microsoft, Salesforce, SAP, and ServiceNow.

**x402** is an open payment standard built on HTTP 402 for machine-native, internet-native payments. Created by Coinbase and coordinated with Cloudflare via the x402 Foundation. Supports stablecoins on EVM and Solana networks. The v2 release (late 2025) introduced CAIP-based identifiers, a modular SDK architecture, and standards-compliant payment headers.

**ACP (Agentic Commerce Protocol)** is an open standard co-developed by OpenAI and Stripe for connecting buyers, AI agents, and businesses to complete purchases. Powers Instant Checkout in ChatGPT. Currently in beta with date-based version snapshots. Designed to work with any PSP — Stripe provides the first implementation via Shared Payment Token.

**MPP (Machine Payments Protocol)** is an open standard co-authored by Tempo Labs and Stripe for machine-to-machine payments over HTTP 402. Supports stablecoins, cards, and bank transfers. Offers `charge` (one-off) and `session` (streaming micropayment) intents. Backwards-compatible with x402. Based on an IETF-proposed Payment HTTP Authentication Scheme. Launched March 2026.

**Trusted Agent Protocol (Visa) / Agent Pay (Mastercard)** help merchants and networks recognize cryptographically verified AI agents during browse and pay flows, built on Web Bot Auth (IETF drafts).

---

## 📄 License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under [CC0 1.0](LICENSE) (Public Domain). No rights reserved.

---

**Keywords:** `ucp` `ap2` `agent-payments` `agentic-commerce` `a2a` `x402` `acp` `mpp` `machine-payments-protocol` `trusted-agent-protocol` `agent-pay` `web-bot-auth` `mcp` `stablecoins` `verifiable-credentials` `google-cloud` `coinbase` `stripe` `openai` `tempo`