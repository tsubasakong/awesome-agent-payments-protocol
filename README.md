# Awesome Agent Payments Protocol [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🚀 Curated resources for **Google's Agent Payments Protocol (AP2)**, **A2A (Agent-to-Agent)**, **x402**, and adjacent **agentic commerce** standards (ACP, Visa/Mastercard trust rails, Web Bot Auth).

**PRs welcome!** Found something amazing? [Open a PR](../../pulls) or [suggest a resource](../../issues/new?template=add_resource.yml) 🎯

_Last updated: 2025-11-06_

---

## 📋 Contents

- [Official Documentation](#-official-documentation)
- [Specifications & Whitepapers](#-specifications--whitepapers)
- [Developer Tools & Starters](#-developer-tools--starters)
- [Ecosystem & Partners](#-ecosystem--partners)
- [News & Analysis](#-news--analysis)
- [Videos & Tutorials](#-videos--tutorials)
- [Community](#-community)

---

## 📚 Official Documentation

### AP2 (Agent Payments Protocol)
- [AP2 Protocol Documentation](https://ap2-protocol.org/) - Overview, mandate types, A2A/MCP relationships, and integrations
- [Google Cloud AP2 Announcement](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol)
- [AP2 GitHub Repository](https://github.com/google-agentic-commerce/AP2)
- [AP2 Specification](https://ap2-protocol.org/specification/)

### A2A (Agent-to-Agent Protocol)
- [A2A Protocol Overview](https://developers.googleblog.com/en/a2a-a-new-era-of-agent-interoperability/)
- [A2A x402 Extension (GitHub)](https://github.com/google-agentic-commerce/a2a-x402)
- [ADK A2A Guides](https://google.github.io/adk-docs/a2a/)
- [A2A Project (Linux Foundation)](https://www.linuxfoundation.org/press/linux-foundation-launches-the-agent2agent-protocol-project-to-enable-secure-intelligent-communication-between-ai-agents)

### x402 (Machine Payments over HTTP 402)
- [x402 Developer Docs](https://docs.cdp.coinbase.com/x402/welcome)
- [x402 Protocol (GitHub)](https://github.com/coinbase/x402)
- [x402 Whitepaper (PDF)](https://www.x402.org/x402-whitepaper.pdf)
- [Coinbase: AP2 + x402 Launch Post](https://www.coinbase.com/developer-platform/discover/launches/google_x402)
- [x402 Product Page](https://www.coinbase.com/developer-platform/products/x402)

### ACP (Agentic Commerce Protocol) - NEW ⭐
- [ACP Overview (OpenAI Developers)](https://developers.openai.com/commerce/)
- [ACP Spec Site](https://agenticcommerce.dev/)
- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol)
- [OpenAI - Buy it in ChatGPT](https://openai.com/index/buy-it-in-chatgpt/)

### Network Trust Rails for Agents - NEW ⭐

#### Visa Trusted Agent Protocol
- [Press Release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare Press Note](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)

#### Mastercard Agent Pay
- [Press Release (Sep 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/september/mastercard-unveils-new-tools-and-collaborations-to-power-smarter%2C-safer-agentic-commerce.html)
- [Initial Announcement (Apr 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai.html)

### Identity / Interop
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) - Standard for AI agent interoperability
- [Web Bot Auth (Cloudflare)](https://developers.cloudflare.com/bots/reference/bot-verification/web-bot-auth/) - Agent identity via HTTP Message Signatures

---

## 📄 Specifications & Whitepapers

### x402 Protocol
- [x402 Whitepaper (PDF)](https://www.x402.org/x402-whitepaper.pdf)
- [x402 Spec & Reference (GitHub)](https://github.com/coinbase/x402)

### A2A & AP2
- [A2A Project (Linux Foundation)](https://www.linuxfoundation.org/press/linux-foundation-launches-the-agent2agent-protocol-project-to-enable-secure-intelligent-communication-between-ai-agents)
- [AP2 Specification](https://ap2-protocol.org/specification/)

### Web Bot Auth / Agent Identity
- [IETF Draft - Web Bot Auth Architecture](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-architecture)

### Research Papers
- "Towards Multi-Agent Economies: A2A + x402 Micropayments" - Proposes ledger-anchored identities with x402 for A2A micropayments

---

## 🛠 Developer Tools & Starters

### AP2 Implementation
- [AP2 Python & Android Samples](https://github.com/google-agentic-commerce/AP2)

### x402 Implementation

#### Quickstarts
- [Quickstart for Sellers](https://docs.cdp.coinbase.com/x402/quickstart-for-sellers)
- [Quickstart for Buyers](https://docs.cdp.coinbase.com/x402/quickstart-for-buyers)
- [MCP Server with x402](https://docs.cdp.coinbase.com/x402/mcp-server)
- [QuickNode - Using x402 for Paywalls](https://www.quicknode.com/guides/infrastructure/how-to-use-x402-payment-required)
- [Crossmint x402 Starter](https://github.com/Crossmint/crossmint-402-starter)

#### SDKs & Libraries
- [x402 Rust crates + Facilitator](https://github.com/x402-rs/x402-rs)
- [Coinbase x402 Repository](https://github.com/coinbase/x402)

### ACP Implementation
- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started/)
- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol)

### Agent Frameworks

#### Cloudflare Agents SDK - NEW ⭐
- [x402 in Agents SDK](https://developers.cloudflare.com/agents/x402/) - Built-in x402 support
- [Agents SDK Overview](https://developers.cloudflare.com/agents/)
- [Cloudflare x402 Foundation Announcement](https://blog.cloudflare.com/x402/)

#### MCP Integration
- [OpenAI Agents SDK - MCP](https://openai.github.io/openai-agents-python/mcp/)

---

## 🌐 Ecosystem & Partners

### x402 Foundation - NEW ⭐
**Cloudflare + Coinbase**: Coordinating adoption of x402. Agents SDK & MCP servers support x402 out of the box. Proposal for **deferred x402 payments** to support aggregation or card rails alongside stablecoins.

### AP2 Partner Ecosystem
**Officially reported supporters**: Shopify, Etsy, Salesforce, Mastercard, PayPal, American Express, Adyen, Worldpay, and 60+ partners total.

### Agent Trust Rails
**Visa's Trusted Agent Protocol** and **Mastercard's Agent Pay** both leverage **Web Bot Auth** for cryptographically signed agent identity during browse and payment flows.

### E-commerce Platforms
- **Shopify** - AP2 & ACP support
- **Etsy** - Live with ACP (Instant Checkout in ChatGPT)
- **Salesforce** - AP2 integration

### Crypto & Web3
- **Coinbase** - x402 creator, AP2 partner
- **Ethereum Foundation** - A2A & x402 collaboration
- **MetaMask** - AP2 ecosystem participant

### Payments Networks
- **Visa** - Trusted Agent Protocol
- **Mastercard** - Agent Pay
- **PayPal** - AP2 support
- **American Express** - AP2 partner
- **Adyen** - AP2 integration
- **Worldpay** - AP2 support

### AI/Agent Platforms
- **OpenAI** - ACP creator (with Stripe)
- **Anthropic** - AP2 ecosystem
- **Google Cloud** - AP2 creator

---

## 📰 News & Analysis

### Major Launches & Announcements

#### AP2 Launch (September 2025)
- [TechCrunch: Google launches new protocol for agent-driven purchases](https://techcrunch.com/2025/09/16/google-launches-new-protocol-for-agent-driven-purchases/)
- [Axios: Google's AP2 aims to boost trust in agent shopping](https://www.axios.com/2025/09/16/google-ai-agents-ecommerce-online-shopping)
- [Digital Commerce 360: AP2 gains support from Shopify, Etsy](https://www.digitalcommerce360.com/2025/09/19/google-ai-payments-protocol-ap2/)
- [The Block: Google launches AI agent-to-agent payments with stablecoin support](https://www.theblock.co/post/370871/google-launches-ai-agent-to-agent-payments-protocol-with-stablecoin-support)

#### OpenAI Instant Checkout & ACP - NEW ⭐
- [Reuters: OpenAI partners with Etsy, Shopify for ChatGPT checkout](https://www.reuters.com/world/americas/openai-partners-with-etsy-shopify-chatgpt-checkout-2025-09-29/)
- [AP News: OpenAI Instant Checkout coverage](https://apnews.com/article/openai-chatgpt-shopping-etsy-shopify)

#### x402 Foundation - NEW ⭐
- [Cloudflare Blog: x402 Foundation announcement](https://blog.cloudflare.com/x402/)
- [The Block: x402 Foundation recap](https://www.theblock.co/post/cloudflare-coinbase-x402-foundation)

#### Network Trust Rails - NEW ⭐
- [Visa: Trusted Agent Protocol press release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare: Collaboration with payments companies](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)
- [Digital Commerce 360: Network trust rails wrap-up](https://www.digitalcommerce360.com/2025/10/15/visa-mastercard-agent-commerce/)

### Industry Analysis
- [Constellation Research: Google's AP2 fleshes out AI agent commerce](https://www.constellationr.com/blog-news/insights/googles-agent-payments-protocol-fleshes-out-ai-agent-commerce)
- [Performance Marketing World: Google & Web3 teams launch x402 extension](https://www.performancemarketingworld.com/article/1932704/google-launches-open-protocol-enable-secure-ai-agent-led-payments)
- [Finextra Deep Dive: Google's AP2 explained](https://www.finextra.com/blogposting/29408/deep-dive-googles-ap2-explained---the-rulebook-for-agent-led-payments)
- [PYMNTS: Google unveils payment protocol for AI-driven commerce](https://www.pymnts.com/artificial-intelligence-2/2025/google-unveils-a-payment-protocol-for-ai-driven-commerce/)

### Security & Standards
- [Cloud Security Alliance: Secure Use of AP2](https://cloudsecurityalliance.org/blog/2025/10/06/secure-use-of-the-agent-payments-protocol-ap2-a-framework-for-trustworthy-ai-driven-transactions) - Security model & guidance
- [PayPal Dev Blog: AP2 mandates as W3C VCs](https://developer.paypal.com/community/blog/PayPal-Agent-Payments-Protocol/) - Technical deep dive

---

## 🎥 Videos & Tutorials

### AP2
- [Intro to Google Agent Payments Protocol (AP2)](https://www.youtube.com/watch?v=yLTp3ic2j5c) - Beginner-friendly introduction
- [AP2 Overview & Ecosystem Breakdown](https://www.youtube.com/watch?v=m03UOWQIiJo) - Comprehensive ecosystem analysis
- [Technical Review: AP2 Code Walkthrough (Kotlin)](https://www.youtube.com/watch?v=5-B86E6w2t4) - Code implementation review
- [AP2 Core Concept: Signed Authorization & Accountability](https://www.youtube.com/shorts/OUITfQDEn3k) - Short-form explanation
- [After MCP & A2A, Meet AP2](https://www.youtube.com/watch?v=vxRe33XUMQY) - Protocol evolution overview

### x402
- [x402 Deep Dive & Demos](https://www.youtube.com/watch?v=pL5LxhZ8iCY) - Technical walkthrough
- [x402 Short Explainer](https://www.youtube.com/shorts/tgpVtCdu3tU) - Quick overview

### ACP
- [OpenAI: Buy it in ChatGPT (ACP)](https://openai.com/index/buy-it-in-chatgpt/) - Official product demo

---

## 💬 Community

### Discussion & Support
- [Google Developers Community: AP2 Introduction](https://discuss.google.dev/t/new-agent-payments-protocol-ap2-an-open-and-secure-standard-for-agentic-payments/265614) - Official community discussion
- [x402 Community FAQ](https://docs.cdp.coinbase.com/x402/support/faq) - FAQ & Discord links

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

**AP2 (Agent Payments Protocol)** is Google's open protocol for agent-driven payments with verifiable authorization (mandates) and accountability. It supports cards, real-time transfers, and stablecoins, and integrates with A2A/MCP patterns.

**x402** is Coinbase's open payment protocol built on HTTP 402 to enable machine-native, programmatic, stablecoin payments. Now stewarded with Cloudflare via the x402 Foundation.

**ACP (Agentic Commerce Protocol)** is OpenAI+Stripe's open standard for agentic commerce, powering Instant Checkout in ChatGPT. Designed to interoperate with existing commerce stacks and payment providers.

**Trusted Agent Protocol / Agent Pay** help merchants and networks recognize cryptographically signed "good agents" during browse and pay flows, built on Web Bot Auth.

---

## 📄 License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under [CC0 1.0](LICENSE) (Public Domain). No rights reserved.

---

**Keywords:** `ap2` `agent-payments` `agentic-commerce` `a2a` `x402` `acp` `trusted-agent-protocol` `agent-pay` `web-bot-auth` `mcp` `stablecoins` `verifiable-credentials` `google-cloud` `coinbase` `stripe` `openai`