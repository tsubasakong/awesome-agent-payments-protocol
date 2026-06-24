# Awesome Agent Payments Protocol [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🚀 Curated resources for the **agentic commerce** protocol landscape — **UCP**, **AP2**, **A2A**, **x402**, **ACP**, **MPP**, trust rails, and interop standards.

**PRs welcome!** Found something amazing? [Open a PR](../../pulls) or [suggest a resource](../../issues/new?template=add_resource.yml) 🎯

*Last updated: 2026-06-07*

---

## 📋 Contents

- [Official Documentation](#-official-documentation)
  - [UCP (Universal Commerce Protocol)](#ucp-universal-commerce-protocol)
  - [AP2 (Agent Payments Protocol)](#ap2-agent-payments-protocol)
  - [A2A (Agent-to-Agent Protocol)](#a2a-agent-to-agent-protocol)
  - [x402 (Machine Payments over HTTP 402)](#x402-machine-payments-over-http-402)
  - [ACP (Agentic Commerce Protocol)](#acp-agentic-commerce-protocol)
  - [MPP (Machine Payments Protocol)](#mpp-machine-payments-protocol)
  - [AMP (Agentic Mobile Protocol)](#amp-agentic-mobile-protocol)
  - [ERC-8183 (Agentic Commerce Escrow)](#erc-8183-agentic-commerce-escrow)
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
- [UCP at Google Marketing Live (May 2026)](https://blog.google/products-and-platforms/products/shopping/shopping-updates-google-marketing-live/) — Universal Cart across Search, Gemini, and Maps with one-tap checkout via Google Pay

### AP2 (Agent Payments Protocol)

- [AP2 Protocol Documentation](https://ap2-protocol.org/) — Overview, mandate types, A2A/MCP relationships, and integrations
- [AP2 Specification](https://ap2-protocol.org/specification/)
- [AP2 GitHub Repository](https://github.com/google-agentic-commerce/AP2) — Spec, Python & Android samples
- [Google Cloud AP2 Announcement](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol)
- [AP2 Roadmap](https://ap2-protocol.org/) — See roadmap section on official site
- [AP2 Partners](https://ap2-protocol.org/) — See partners section on official site
- [AP2 and UCP](https://ap2-protocol.org/) — How AP2 provides the payment mandate layer for UCP
- [Google Gemini Spark](https://tech.yahoo.com/ai/gemini/articles/googles-gemini-spark-announced-meet-174500393.html) — Always-on consumer agent (Gemini 3.5) that queues, monitors, and finalizes purchases under AP2 guardrails (spend caps, merchant allow-lists, explicit approval, permanent transaction trail); announced at Google I/O 2026

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
>
> **Status update (Mar 2026):** OpenAI discontinued the consumer-facing **Instant Checkout** experience in ChatGPT after a ~5-month trial (low adoption, weak conversion, unresolved sales-tax handling). The **ACP protocol itself continues** in a narrower form, with OpenAI refocusing on product discovery and ChatGPT apps; Stripe and PayPal remain involved on the payments side. See News & Analysis below.

- [ACP Spec Site](https://agenticcommerce.dev/) — Protocol overview and interactive demo
- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started)
- [ACP: Key Concepts](https://developers.openai.com/commerce/) — Protocol page on OpenAI Developers
- [ACP: Product Feeds](https://developers.openai.com/commerce/) — Product feed spec for merchant integration
- [ACP: Agentic Checkout Spec](https://developers.openai.com/commerce/) — Checkout flow and endpoints
- [ACP: Delegated Payment Spec](https://developers.openai.com/commerce/) — Shared Payment Token and PSP integration
- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) — Spec, RFCs, examples, changelog
- [OpenAI: Buy it in ChatGPT](https://openai.com/index/buy-it-in-chatgpt/) — Instant Checkout launch post (Sep 2025; consumer feature later discontinued — see News)

#### Stripe ACP / Agentic Commerce Resources

- [Stripe: Integrate the ACP](https://docs.stripe.com/agentic-commerce/protocol) — RESTful or MCP server implementation guide
- [Stripe: Shared Payment Token](https://docs.stripe.com/agentic-commerce/) — Payment primitive for agentic flows
- [Stripe Blog: Developing an Open Standard for Agentic Commerce](https://stripe.com/blog/developing-an-open-standard-for-agentic-commerce)

### MPP (Machine Payments Protocol)

- [MPP Official Site](https://mpp.dev/overview) — Protocol overview, SDKs, and quickstart
- [Stripe: Machine Payments with MPP](https://docs.stripe.com/payments/machine/mpp) — Implementation docs (crypto + fiat via PaymentIntents)
- [Stripe Blog: Introducing MPP](https://stripe.com/blog/machine-payments-protocol) — Launch post (Mar 2026)
- [Cloudflare Agents Docs: MPP](https://developers.cloudflare.com/agents/agentic-payments/mpp/) — MPP integration in Cloudflare Workers
- [Visa: Card Specification & SDK for MPP](https://corporate.visa.com/en/sites/visa-perspectives/innovation/visa-card-specification-sdk-for-machine-payments-protocol.html) — Openly available, processor-agnostic card-based MPP spec + SDK; passes tokenized card credentials through MPP workflows; ties into Visa Intelligent Commerce and Trusted Agent Protocol (2026)
- [IETF Draft: Payment HTTP Authentication Scheme](https://mpp.dev/overview) — See spec link on mpp.dev

> **MPP and x402:** MPP is backwards-compatible with x402. The core x402 exact-payment flows map directly onto MPP's `charge` intent, so MPP clients can consume existing x402 services without modification. MPP additionally supports `session` (streaming/pay-as-you-go) payments, recurring payments, and microtransactions across stablecoins, cards, and bank transfers.

### AMP (Agentic Mobile Protocol)

- [Ant International: AMP Launch (Business Wire)](https://www.businesswire.com/news/home/20260427209524/en/Ant-International-Launches-Open-Sourced-Agentic-Mobile-Protocol-to-Drive-AI-Commerce) — World's first open-sourced agentic payment framework for mobile surfaces (digital wallets, super apps, banking apps, wearables, in-car), announced Apr 28, 2026
- Connects LLMs, platforms, and merchant agents to 4.4B+ digital wallet users via Alipay+; cuts agent-to-wallet linking steps ~50% vs card binding; per-transaction money-back guarantee for account-takeover cases

### ERC-8183 (Agentic Commerce Escrow)

- [ERC-8183 Specification](https://eips.ethereum.org/EIPS/eip-8183) — Official EIP
- [ERC-8183 Discussion](https://ethereum-magicians.org/t/erc-8183-agentic-commerce/27902) — Ethereum Magicians thread
- [ERC-8004 Specification](https://eips.ethereum.org/EIPS/eip-8004) — Companion identity + reputation registries that ERC-8183 contracts can write feedback to on settlement

> **ERC-8183 vs x402 / MPP:** Where x402 and MPP settle instantly per request (good for stateless metered access), ERC-8183 is the **on-chain escrow** standard for *service-delivery* between agents — cases where the deliverable can't be verified by HTTP 200 and a neutral Evaluator may need to adjudicate. Lifecycle: `createJob → approve → fund → submit → complete | reject`. Stablecoin-denominated, 3-way fee split (provider/evaluator/platform) enforced by the contract, refund-on-expiry, native composition with ERC-8004 reputation feedback on settlement.

### Network Trust Rails for Agents

#### Visa Trusted Agent Protocol

- [Press Release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare Press Note](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)
- [Visa Agentic Ready Program — LatAm & Asia expansion (Apr 2026)](https://www.digitalcommerce360.com/2026/04/02/visa-mastercard-in-agentic-commerce/) — Geographic expansion plus AI-assisted disputes and a Ramp partnership for automated corporate bill pay

#### Mastercard Agent Pay

- [Press Release (Sep 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/september/mastercard-unveils-new-tools-and-collaborations-to-power-smarter%2C-safer-agentic-commerce.html)
- [Initial Announcement (Apr 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai.html)
- [Agent Pay international expansion, incl. Hong Kong (2026)](https://www.americanbanker.com/payments/news/visa-mastercard-expand-agentic-ai-deployments) — Part of Mastercard's push toward an international agentic-commerce network

### Identity / Interop

- [Model Context Protocol (MCP) — Spec & Docs](https://modelcontextprotocol.io/) — Standard for AI agent tool interoperability
- [MCP Specification (GitHub)](https://github.com/modelcontextprotocol/specification) — Protocol spec repository
- [MCP Registry (Preview)](https://github.com/mcp) — GitHub MCP Registry for discovering MCP servers
- [Web Bot Auth — Architecture Draft (IETF)](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-architecture) — Agent identity via HTTP Message Signatures
- [Web Bot Auth — Directory Draft (IETF)](https://datatracker.ietf.org/doc/html/draft-meunier-web-bot-auth-directory) — Directory for verified bot identities
- [Web Bot Auth (Cloudflare Developer Docs)](https://developers.cloudflare.com/bots/reference/bot-verification/web-bot-auth/)
- [ZKProofport](https://zkproofport.app) — Zero-knowledge proof generation for AI agent identity. Lets agents prove Coinbase KYC, Country, Google OIDC, Google Workspace, or Microsoft 365 affiliation via x402-paid TEE proving on Base. ERC-8004 registered, A2A compatible. NPM: `@zkproofport-ai/mcp`. Reference app: [OpenStoa](https://github.com/zkproofport/openstoa) (1st place — The Synthesis Hackathon 2026)

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

### ERC-8183 / ERC-8004

- [ERC-8183 — Agentic Commerce](https://eips.ethereum.org/EIPS/eip-8183) — On-chain escrow standard for agent-to-agent service delivery (lifecycle, fee splits, evaluator role, expiry refund)
- [ERC-8004 — Trustless Agents](https://eips.ethereum.org/EIPS/eip-8004) — On-chain identity and reputation registries for autonomous agents (signed feedback, scoring rules hash, ERC-1271 contract signatures)

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
- [x402 Wallet for Claude Desktop](https://github.com/402md/x402-wallet-for-claude-desktop) — Claude Desktop extension with x402 USDC payments on Stellar and Base. Automatic 402 handling with configurable spending limits.

#### Live Services

- [PoolPulse](https://poolpulse.poolpulse.workers.dev) — x402-payable DeFi execution signals API on Base. CLMM slippage, MEV scoring, routing hints for 33 Uniswap V3 + Aerodrome pools. Built with Hono + x402/hono. Pay per call ($0.001–$0.25 USDC). ([OpenAPI](https://poolpulse.poolpulse.workers.dev/openapi.json), [Examples](https://github.com/HadiFrt20/poolpulse-agent-example))
- [Coinbase x402 Bazaar](https://docs.cdp.coinbase.com/x402/bazaar) — Discovery layer / MCP server exposing 10,000+ x402-payable endpoints that agents can search, discover, and pay for autonomously (also surfaced via AWS Bedrock AgentCore Gateway)

#### SDKs & Libraries

- [x402 Monorepo (GitHub)](https://github.com/coinbase/x402) — `@x402/core`, `@x402/evm`, `@x402/svm`, `@x402/axios`, `@x402/fetch`, `@x402/express`, `@x402/hono`, `@x402/next`, `@x402/paywall`
- [x402 Rust crates + Facilitator](https://github.com/x402-rs/x402-rs)
- [x402-proxy](https://github.com/cascade-protocol/x402-proxy) — `curl` for x402 paid APIs. Auto-pays HTTP 402 responses with USDC, with MCP stdio proxy for AI agents

### ACP Implementation

- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started/)
- [ACP Spec & Examples (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol)
- [Stripe: Integrate the ACP](https://docs.stripe.com/agentic-commerce/protocol)

### MPP Implementation

- [MPP SDKs](https://mpp.dev/overview) — Official TypeScript SDK (`mppx`) with middleware for Hono, Express, Next.js, Elysia
- [Stripe: Machine Payments with MPP](https://docs.stripe.com/payments/machine/mpp) — Implementation with PaymentIntents
- [Visa Card Spec & SDK for MPP](https://corporate.visa.com/en/sites/visa-perspectives/innovation/visa-card-specification-sdk-for-machine-payments-protocol.html) — Card-based MPP transactions via tokenized network payment tokens settling over existing card infrastructure

### A2A Implementation

- [A2A Samples Repository](https://github.com/a2aproject/a2a-samples) — Hello-world, multi-agent, and framework-specific examples
- [A2A Inspector](https://github.com/a2aproject/a2a-inspector) — Validate your A2A agent

### ERC-8183 / ERC-8004 Implementation

- [CardZero](https://cardzero.ai) — First known production deployment of ERC-8004 + ERC-8183 on Base mainnet. ERC-4337 smart-contract wallet for AI agents with owner-set spending rules, x402 buyer support, and full Job-escrow lifecycle live at `api.cardzero.ai/v1/jobs`. Source on [GitHub](https://github.com/mrocker/CardZero); MCP server published as [`cardzero-mcp`](https://www.npmjs.com/package/cardzero-mcp); 27-page docs + `/llms-full.txt` corpus at [cardzero.ai/docs](https://cardzero.ai/docs).

### Agent Frameworks & Managed Platforms

#### Amazon Bedrock AgentCore Payments

- [AWS What's New: AgentCore Payments (preview)](https://aws.amazon.com/about-aws/whats-new/2026/04/amazon-bedrock-agentcore-payments-preview/) — Managed surface for agents to pay for APIs, MCP servers, web content, and other agents
- [AWS ML Blog: Agents that transact (built with Coinbase and Stripe)](https://aws.amazon.com/blogs/machine-learning/agents-that-transact-introducing-amazon-bedrock-agentcore-payments-built-with-coinbase-and-stripe/) — Wraps x402 negotiation, wallet auth, stablecoin settlement, and proof delivery; deterministic session spending limits at the infra layer
- [Coinbase Blog: AgentCore Payments powered by x402](https://www.coinbase.com/blog/introducing-amazon-bedrock-agentcore-payments-powered-by-x402-and-coinbase)
- [Sample: AgentCore + CloudFront + x402](https://github.com/aws-samples/sample-agentcore-cloudfront-x402-payments) — Reference demo using Bedrock AgentCore, Strands SDK, and CloudFront

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

Co-developed by **Google** and **Shopify**. Endorsed by 20+ partners including Etsy, Wayfair, Target, Walmart, Adyen, American Express, Best Buy, Flipkart, Macy's Inc., Mastercard, Stripe, The Home Depot, Visa, and Zalando. ([Source: Google Blog, Jan 2026](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/)). May 2026: Universal Cart extends checkout across Search, Gemini, and Maps with Google Pay. ([Source: Google Marketing Live](https://blog.google/products-and-platforms/products/shopping/shopping-updates-google-marketing-live/))

### AP2

Officially reported supporters include Shopify, Etsy, Salesforce, Mastercard, PayPal, American Express, Adyen, Worldpay, and 60+ partners total. ([Source: AP2 Protocol site](https://ap2-protocol.org/))

### x402 Foundation

**Cloudflare + Coinbase** coordinating adoption of x402. The Agents SDK and MCP servers support x402 out of the box. x402 v2 adds modular payment scheme support for EVM and Solana networks. As of mid-2026, **AWS Bedrock AgentCore** also wraps x402 as a managed payment surface (built with Coinbase and Stripe), and the **Coinbase x402 Bazaar** exposes 10,000+ payable endpoints. Per Chainalysis, x402 surpassed **100M+ agentic transactions on Base** within ~9 months of launch.

### ACP

**OpenAI + Stripe** co-developed ACP. The consumer-facing **Instant Checkout** experience in ChatGPT was **discontinued in early 2026** after a ~5-month trial (low adoption, weak conversion, unresolved sales-tax handling); the **ACP protocol continues** in a narrower form with OpenAI refocusing on product discovery and ChatGPT apps. ACP remains open to any PSP — Stripe provides the first implementation via Shared Payment Token, with PayPal also involved. ([Source: TechCrunch, Mar 2026](https://techcrunch.com/2026/03/24/openais-plans-to-make-chatgpt-more-like-amazon-arent-going-so-well/))

### MPP / Tempo

**Stripe + Tempo Labs (Paradigm)** co-authored MPP. Design partners include Anthropic, DoorDash, Mastercard, Nubank, OpenAI, Ramp, Revolut, Shopify, Standard Chartered, and Visa. Cloudflare supports MPP in its Agents SDK. ([Source: Stripe Blog, Mar 2026](https://stripe.com/blog/machine-payments-protocol))

### AMP / Ant International

Open-sourced by **Ant International** and implemented with **Alipay+** wallet partners (40+ wallets, 1.8B accounts, 150M merchants). AMP targets mobile-native agentic payments across smartphones, smartwatches, AR glasses, and in-car systems. ([Source: Business Wire, Apr 2026](https://www.businesswire.com/news/home/20260427209524/en/Ant-International-Launches-Open-Sourced-Agentic-Mobile-Protocol-to-Drive-AI-Commerce))

### Agent Trust Rails

**Visa's Trusted Agent Protocol** and **Mastercard's Agent Pay** both leverage **Web Bot Auth** for cryptographically signed agent identity during browse and payment flows. In 2026 both expanded internationally — Visa's Agentic Ready program to Latin America and Asia, and Mastercard's Agent Pay to markets including Hong Kong.

### Agent Reputation & Scoring

- [DJD Agent Score](https://djd-agent-score.fly.dev) — Behavioral reputation scoring API for AI agent wallets on Base. Scores agents 0–100 across 5 dimensions using on-chain transaction patterns, sybil detection, and gaming velocity checks. x402-native monetization, MCP server distribution, and ERC-8004 compatible. ([GitHub](https://github.com/jacobsd32-cpu/djd-agent-score))

### Analytics & Dashboards

- [agenteconomy.to](https://agenteconomy.to) — Real-time dashboard tracking AI agent on-chain payment activity across x402, ERC-8004, ERC-8183 (Virtuals ACP), and MPP (Stripe/Tempo) on 8 chains. Aggregated event counter, chain distribution, facilitator share, and time-series charts. Data refreshes every 6 hours. ([source](https://github.com/realdora/agenteconomy))

### Payments Networks

- **Visa** — Trusted Agent Protocol; Agentic Ready program (expanded to LatAm & Asia, 2026); card specification + SDK extending MPP to card payments (2026)
- **Mastercard** — Agent Pay (international expansion incl. Hong Kong, 2026); acquired BVNK for stablecoin infrastructure
- **PayPal** — AP2 support; ACP participant; upcoming UCP payment method
- **American Express** — AP2 partner, UCP endorser
- **Adyen** — AP2 integration, UCP endorser
- **Worldpay** — AP2 support
- **Stripe** — ACP co-creator, MPP co-author, UCP endorser
- **AWS** — Bedrock AgentCore Payments (preview), managed x402 + Stripe surface built with Coinbase and Stripe

### Stablecoin & Settlement Infrastructure

- **AllUnity** — Launched an agentic payments settlement layer powered by x402; planning a Swedish krona stablecoin (SEKAU, MiCA-regulated e-money token) targeting a June 2026 debut, settling AI-initiated transactions into local bank accounts ([CoinDesk](https://www.coindesk.com/business/2026/05/20/germany-s-allunity-plans-swedish-krona-stablecoin-pushes-into-ai-agentic-payments))
- **Fireblocks** — Agentic Payments Suite for stablecoin transactions ([The Paypers](https://thepaypers.com/payments/news/fireblocks-launches-agentic-payments-suite-for-stablecoin-transactions))
- **Circle + Nium** — Partnership to strengthen stablecoin rails for agentic AI payments ([American Banker](https://www.americanbanker.com/payments/news/circle-and-nium-partner-to-boost-stablecoins-ai))

### AI / Agent Platforms

- **Google Cloud** — AP2 creator, UCP co-developer
- **OpenAI** — ACP co-creator (with Stripe)
- **Anthropic** — MPP design partner
- **Shopify** — UCP co-developer, AP2 & ACP partner
- **AWS** — Bedrock AgentCore Payments (x402 + Stripe), with the x402 Bazaar MCP server via AgentCore Gateway

### Crypto & Web3

- **Coinbase** — x402 creator, AP2 partner, AgentCore Payments partner
- **Tempo Labs** — MPP co-author (Paradigm-backed, payments-optimized L1)
- **Radius Network** — x402-compatible stablecoin L1 for agentic micropayments (mainnet launched Mar 2026; sub-second finality, sub-penny fees) ([docs](https://docs.radiustech.xyz/developer-resources/x402-integration))

---

## 📰 News & Analysis

### Major Launches & Milestones

#### Amazon Bedrock AgentCore Payments (Preview, May 2026)

- [AWS What's New: AgentCore Payments (preview)](https://aws.amazon.com/about-aws/whats-new/2026/04/amazon-bedrock-agentcore-payments-preview/)
- [AWS ML Blog: Agents that transact, built with Coinbase and Stripe](https://aws.amazon.com/blogs/machine-learning/agents-that-transact-introducing-amazon-bedrock-agentcore-payments-built-with-coinbase-and-stripe/)
- [Coinbase Blog: AgentCore Payments powered by x402](https://www.coinbase.com/blog/introducing-amazon-bedrock-agentcore-payments-powered-by-x402-and-coinbase)

#### Google Gemini Spark (Google I/O, May 2026)

- [Gemini Spark announced (Yahoo Tech)](https://tech.yahoo.com/ai/gemini/articles/googles-gemini-spark-announced-meet-174500393.html) — Consumer AP2 agent surface with autonomous, guardrailed purchasing
- [Google I/O 2026 recap (TheTechHacker)](https://thetechhacker.com/2026/05/20/google-io-2026-recap-gemini-flash-autonomous-agent/)

#### Ant International Launches AMP (April 2026)

- [Business Wire: Ant International launches open-sourced Agentic Mobile Protocol](https://www.businesswire.com/news/home/20260427209524/en/Ant-International-Launches-Open-Sourced-Agentic-Mobile-Protocol-to-Drive-AI-Commerce) — Mobile-native agentic payments via Alipay+

#### OpenAI Discontinues Instant Checkout (Q1 2026)

- [TechCrunch: OpenAI's plans to make ChatGPT more like Amazon aren't going so well](https://techcrunch.com/2026/03/24/openais-plans-to-make-chatgpt-more-like-amazon-arent-going-so-well/)
- [CNBC: OpenAI's first crack at online shopping stumbled — preparing for the next wave](https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html)

#### UCP Launch & Expansion (Jan–May 2026)

- [Google Blog: New tech and tools for retailers (NRF 2026)](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/)
- [Google Developers Blog: Under the Hood of UCP](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/)
- [UCP Updates: Multi-item carts, catalog, identity linking (Mar 2026)](https://blog.google/products-and-platforms/products/shopping/ucp-updates/)
- [UCP at Google Marketing Live: Universal Cart (May 2026)](https://blog.google/products-and-platforms/products/shopping/shopping-updates-google-marketing-live/)

#### A2A v1.0 (2026)

- [A2A: Announcing Version 1.0](https://a2a-protocol.org/latest/announcing-1.0/) — Enterprise features, signed agent cards, multi-tenancy

#### MPP Launch (March 2026)

- [Stripe Blog: Introducing MPP](https://stripe.com/blog/machine-payments-protocol)
- [Cloudflare Agents Docs: MPP](https://developers.cloudflare.com/agents/agentic-payments/mpp/)

#### x402 V2 & Adoption (Late 2025 – 2026)

- [x402 V2 Launch Post](https://www.x402.org/writing/x402-v2-launch)
- [Cloudflare Agents SDK v0.4.0: x402 v2 migration](https://developers.cloudflare.com/changelog/post/2026-02-09-agents-sdk-v040/)
- [Agentic payments surpass 100M transactions on Base (Chainalysis)](https://www.cryptobreaking.com/agentic-payments-surpass-100m-transactions/)

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

#### Network Trust Rails (2025–2026)

- [Visa: Trusted Agent Protocol press release](https://investor.visa.com/news/news-details/2025/Visa-Introduces-Trusted-Agent-Protocol-An-Ecosystem-Led-Framework-for-AI-Commerce/default.aspx)
- [Cloudflare: Collaboration with payments companies](https://www.cloudflare.com/press/press-releases/2025/cloudflare-collaborates-with-leading-payments-companies-to-secure-and-enable-agentic-commerce/)
- [Visa & Mastercard expand agentic AI deployments (American Banker, 2026)](https://www.americanbanker.com/payments/news/visa-mastercard-expand-agentic-ai-deployments)
- [How Visa and Mastercard are approaching agentic commerce (Digital Commerce 360, Apr 2026)](https://www.digitalcommerce360.com/2026/04/02/visa-mastercard-in-agentic-commerce/)

### Industry Analysis

- [Constellation Research: Google's AP2 fleshes out AI agent commerce](https://www.constellationr.com/blog-news/insights/googles-agent-payments-protocol-fleshes-out-ai-agent-commerce)
- [Finextra Deep Dive: Google's AP2 explained](https://www.finextra.com/blogposting/29408/deep-dive-googles-ap2-explained---the-rulebook-for-agent-led-payments)
- [PYMNTS: Google unveils payment protocol for AI-driven commerce](https://www.pymnts.com/artificial-intelligence-2/2025/google-unveils-a-payment-protocol-for-ai-driven-commerce/)
- [Digital Commerce 360: OpenAI expands agentic commerce push (Feb 2026)](https://www.digitalcommerce360.com/2026/02/16/openai-expands-agentic-commerce-push/)
- [Forrester: Agentic Payments in B2C Commerce — Where We Are Now](https://www.forrester.com/blogs/agentic-payments-in-b2c-commerce-where-we-are-now/)
- [PYMNTS: Payment Networks Ready Infrastructure for Agentic Commerce at Scale](https://www.pymnts.com/news/artificial-intelligence/2026/payment-networks-ready-infrastructure-agentic-commerce-scale/)
- [Fenwick: Is 2026 the Year of Agentic Payments?](https://www.fenwick.com/insights/publications/is-2026-the-year-of-agentic-payments)

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

**UCP (Universal Commerce Protocol)** is an open standard co-developed by Google and Shopify for agentic commerce across the full shopping journey — discovery, checkout, identity linking, and order management. UCP is transport-agnostic (REST, MCP, A2A) and compatible with AP2 for secure payment mandates. Launched January 2026 at NRF; Universal Cart (checkout across Search, Gemini, and Maps with Google Pay) added May 2026.

**AP2 (Agent Payments Protocol)** is Google's open protocol for agent-driven payments with verifiable authorization (mandates) and accountability. Its current core focus is card-based payments with mandate-driven authorization. AP2 serves as the payment layer within UCP.

**A2A (Agent-to-Agent Protocol)** is an open standard under the Linux Foundation for agent interoperability — discovery, communication, and task delegation across agent frameworks and vendors. The v1.0 release (2026) added enterprise features including signed agent cards, multi-tenancy, and version negotiation. The TSC includes AWS, Cisco, Google, IBM Research, Microsoft, Salesforce, SAP, and ServiceNow.

**x402** is an open payment standard built on HTTP 402 for machine-native, internet-native payments. Created by Coinbase and coordinated with Cloudflare via the x402 Foundation. Supports stablecoins on EVM and Solana networks. The v2 release (late 2025) introduced CAIP-based identifiers, a modular SDK architecture, and standards-compliant payment headers. By mid-2026 it is wrapped by managed surfaces such as AWS Bedrock AgentCore and had surpassed 100M+ agentic transactions on Base.

**ACP (Agentic Commerce Protocol)** is an open standard co-developed by OpenAI and Stripe for connecting buyers, AI agents, and businesses to complete purchases. It originally powered Instant Checkout in ChatGPT; the consumer Instant Checkout experience was discontinued in early 2026, while the ACP protocol continues in a narrower form. Currently in beta with date-based version snapshots. Designed to work with any PSP — Stripe provides the first implementation via Shared Payment Token.

**MPP (Machine Payments Protocol)** is an open standard co-authored by Tempo Labs and Stripe for machine-to-machine payments over HTTP 402. Supports stablecoins, cards, and bank transfers. Offers `charge` (one-off) and `session` (streaming micropayment) intents. Backwards-compatible with x402. Based on an IETF-proposed Payment HTTP Authentication Scheme. Launched March 2026.

**AMP (Agentic Mobile Protocol)** is an open-sourced framework from Ant International for agentic payments on mobile surfaces — digital wallets, super apps, banking apps, and wearables. Implemented via Alipay+, it emphasizes fast agent-to-wallet linking (~50% fewer steps than card binding) and account-takeover protection with a per-transaction money-back guarantee. Launched April 2026.

**Trusted Agent Protocol (Visa) / Agent Pay (Mastercard)** help merchants and networks recognize cryptographically verified AI agents during browse and pay flows, built on Web Bot Auth (IETF drafts). Both expanded internationally in 2026. In 2026 Visa also released an open, processor-agnostic card specification and SDK extending MPP to card payments.

---

## 📄 License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under [CC0 1.0](LICENSE) (Public Domain). No rights reserved.

---

**Keywords:** `ucp` `ap2` `agent-payments` `agentic-commerce` `a2a` `x402` `acp` `mpp` `machine-payments-protocol` `amp` `agentic-mobile-protocol` `trusted-agent-protocol` `agent-pay` `gemini-spark` `web-bot-auth` `mcp` `stablecoins` `verifiable-credentials` `agentcore` `erc-8183` `erc-8004` `google-cloud` `coinbase` `stripe` `openai` `aws` `tempo`


## MetaVision
- [MetaVision AI Platform](https://metavision.click) - Web3 CVE Oracle (355k+ NVD vulnerabilities, $0.50 USDC), DeFi arbitrage signals on Base ($0.10 USDC), wallet fraud + rug pull detection. 18 MCP tools. x402 v2. ([Agent Card](https://metavision.click/.well-known/agent.json))