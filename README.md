# Awesome Agent Payments Protocol [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🚀 Curated resources for the **agentic commerce** protocol landscape — **UCP**, **AP2**, **A2A**, **x402**, **ACP**, **MPP**, trust rails, and interop standards.

**PRs welcome!** Found something amazing? [Open a PR](../../pulls) or [suggest a resource](../../issues/new?template=add_resource.yml) 🎯

*Last updated: 2026-09-22*

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
  - [Agentic Commerce Trust Protocol (Alipay)](#agentic-commerce-trust-protocol-alipay)
  - [ERC-8183 (Agentic Commerce Escrow)](#erc-8183-agentic-commerce-escrow)
  - [Network Trust Rails for Agents](#network-trust-rails-for-agents)
  - [Identity / Interop](#identity--interop)
  - [Accountability & Evidence Layer](#accountability--evidence-layer)
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
- [Introducing the Universal Cart (Google I/O 2026, May 19)](https://blog.google/products-and-platforms/products/shopping/google-shopping-cart/) — Universal Cart across **Search, Gemini, YouTube, and Gmail**; built on Google Wallet (card perks, loyalty, merchant offers); checkout with Google Pay or transfer to the merchant site, with the brand always merchant of record. Live merchants include Nike, Sephora, Target, Ulta Beauty, Walmart, Wayfair, and Shopify merchants such as Fenty and Steve Madden
- [UCP at Google Marketing Live (May 2026)](https://blog.google/products-and-platforms/products/shopping/shopping-updates-google-marketing-live/) — Retailer-facing UCP features and AI tools
- **UCP expansion roadmap (announced May 2026):** UCP-powered checkout extends to **Canada and Australia** in the coming months and to the **U.K.** later; UCP comes to **YouTube** in the U.S.; new verticals begin with **hotel booking and local food delivery**. Universal Cart rolls out across Search and the Gemini app in the U.S. over summer 2026, with YouTube and Gmail to follow
- [Shopify: self-serve UCP agent registration (Jun 17, 2026)](https://www.shopify.com/news/ai-commerce-at-scale) — Shopify opened UCP to all developers: register an agent profile in the Shopify Developer Dashboard and call the public MCP endpoint with **no approval gate** (made self-serve in the Spring '26 Edition)
- [Amazon, Meta, Microsoft, Salesforce, and Stripe join the UCP Tech Council (Apr 24, 2026)](https://ppc.land/amazon-meta-microsoft-salesforce-and-stripe-join-ucp-tech-council/) — Five new members join founders Google, Shopify, Etsy, Target, and Wayfair (now **10**); the Tech Council is UCP's steering body, reviewing technical contribution proposals ([The Paypers](https://thepaypers.com/payments/news/amazon-meta-microsoft-salesforce-and-stripe-join-the-universal-commerce-protocol-council))
- [**UCP v2026-08-25 release (Aug 25, 2026)**](https://github.com/Universal-Commerce-Protocol/ucp/releases/tag/v2026-08-25) — Latest shipped snapshot on the Tech Council's **quarterly release** cadence. Vendor-agnostic **3D Secure (3DS2)** via a new `actions[]` primitive, **Web Bot Auth interop**, a **multi-vertical refactor** (Shopping / Payment / Common namespaces, polymorphic token binding), **grocery readiness** (location search & lookup, operating hours, fractional quantities), **payment terms & schedules** (deferred, deposits, installments), **split payments**, a **loyalty extension**, delegated IdPs, and reverse-DNS buyer consent. Includes **breaking schema changes** (fulfillment restructure, `keys[]` as sole signing-key field, payment extensions moved to `dev.ucp.common.payment.*`) ([ucp.dev announcements](http://ucp.dev/documentation/announcements/))
- **Domain Technical Councils (Jul–Sep 2026):** all three now seated — **Food TC** (Jul 16: Block/Square, DoorDash, Google, Toast, Uber Eats), **Lodging TC** (Aug 11: Amadeus, Booking.com, Expedia, Google, Hilton, Marriott, Trip.com), and **Payments TC** (Sep 2: **Adyen, Ant International, Coinbase, Global Payments, Google, PayPal, Shopify, Stripe**). Stripe also joined the **Governing Council** (Apr 28) alongside permanent members Google and Shopify ([ucp.dev announcements](http://ucp.dev/documentation/announcements/); [Payments TC discussion #798](https://github.com/Universal-Commerce-Protocol/ucp/discussions/798))
- **UCP adoption surge (Sep 2026, independent census):** Shopify's template moved to **v2026-08-25** on Aug 28–29 (~10,600 stores in two days); between **Sep 17–19 Shopify switched on identity linking** (declarations 27 → **7,355**, nearly all delegating to Shop accounts); on **Sep 22 Wix began rolling out cart** across its ~6,929 stores. Census as of Sep 22: **17,767 verified stores**, ~60% on v2026-08-25, **14** commerce platforms with a verified store (up from 6), and the **first production merchant declaring a payment token** (AP2 mandates on the new `common.payment` namespace) ([UCP Checker — State of Agentic Commerce, Sep 2026](https://ucpchecker.com/blog/state-of-agentic-commerce-september-2026))
- **Salesforce Commerce Cloud — UCP GA in October 2026** (announced at Dreamforce, Sep 15): Commerce Cloud merchants get UCP-powered discovery and checkout in Google Search / AI Mode and the Gemini app, with payments and order management kept on the merchant's existing stack ([Salesforce](https://www.salesforce.com/commerce/ai/agentic-commerce/universal-commerce-protocol/); [UCP Checker](https://ucpchecker.com/blog/salesforce-commerce-cloud-ucp-october))

### AP2 (Agent Payments Protocol)

- [AP2 Protocol Documentation](https://ap2-protocol.org/) — Overview, mandate types, A2A/MCP relationships, and integrations
- [AP2 Specification](https://ap2-protocol.org/specification/)
- [AP2 GitHub Repository](https://github.com/google-agentic-commerce/AP2) — Spec, Python & Android samples
- [Google Cloud AP2 Announcement](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol)
- [Google donates AP2 to the FIDO Alliance](https://blog.google/products-and-platforms/platforms/google-pay/agent-payments-protocol-fido-alliance/) — Governance transferred to the **FIDO Alliance** for open, community-led standards (Apr–May 2026); 60+ organizations
- [AP2 v0.2 (GitHub)](https://github.com/google-agentic-commerce/AP2) — v0.2 (Apr 28, 2026) adds **"Human Not Present"** payments and **Verifiable Intent** (a tamper-proof log of user-authorized agent actions, co-developed with Mastercard and also donated to FIDO)
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
- [Linux Foundation: x402 Foundation formation](https://www.linuxfoundation.org/press/linux-foundation-is-launching-the-x402-foundation-and-welcoming-the-contribution-of-the-x402-protocol) — x402 contributed by Coinbase to the **Linux Foundation** for neutral governance (Apr 2026); founding contributors Coinbase, Cloudflare, and Stripe
- [Linux Foundation: x402 Foundation **operational launch** (Jul 14, 2026)](https://www.linuxfoundation.org/press/linux-foundation-announces-operational-launch-of-x402-foundation-to-standardize-internet-native-payments-for-ai-agents-and-applications) — Coinbase's contribution of the protocol **completed**; governance body live with **40 members** across premier and general tiers ([PRNewswire](https://www.prnewswire.com/news-releases/linux-foundation-announces-operational-launch-of-x402-foundation-to-standardize-internet-native-payments-for-ai-agents-and-applications-302824778.html) · [PYMNTS](https://www.pymnts.com/news/2026/40-finance-and-tech-giants-unite-to-standardize-agentic-payments/))
- [Cloudflare Blog: x402 Foundation](https://blog.cloudflare.com/x402/) — Cloudflare's x402 Foundation note (with Coinbase)

### ACP (Agentic Commerce Protocol)

> **Note:** The ACP spec is in **beta** and uses date-based version snapshots (2025-09-29, 2025-12-12, 2026-01-16, 2026-01-30, **2026-04-17**). The current stable snapshot is **2026-04-17** — covers cart, feed, orders, authentication, and MCP, adding capability-negotiation refinements and a seller-backed payment handler. Governed by OpenAI and Stripe as founding maintainers (Apache 2.0) via a SEP (Specification Enhancement Proposal) process, with a stated path toward broader community governance.
>
> **Status update (Mar 2026):** OpenAI discontinued the consumer-facing **Instant Checkout** experience in ChatGPT after a ~5-month trial (low adoption, weak conversion, unresolved sales-tax handling). Rather than shrinking, **ACP changed shape**: OpenAI extended it into a **discovery-and-handoff layer** — merchants share product feeds and promotions so catalogs are represented in ChatGPT, and shoppers are routed to the merchant's own checkout. Stripe and PayPal remain involved on the payments side. See News & Analysis below.

- [ACP Spec Site](https://agenticcommerce.dev/) — Protocol overview and interactive demo
- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started)
- [ACP: Key Concepts](https://developers.openai.com/commerce/) — Protocol page on OpenAI Developers
- [ACP: Product Feeds](https://developers.openai.com/commerce/) — Product feed spec for merchant integration
- [ACP: Agentic Checkout Spec](https://developers.openai.com/commerce/) — Checkout flow and endpoints
- [ACP: Delegated Payment Spec](https://developers.openai.com/commerce/) — Shared Payment Token and PSP integration
- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) — Spec, RFCs, examples, changelog
- [OpenAI: Buy it in ChatGPT](https://openai.com/index/buy-it-in-chatgpt/) — Instant Checkout launch post (Sep 2025; consumer feature later discontinued — see News)
- [OpenAI: Powering Product Discovery in ChatGPT (Mar 24, 2026)](https://openai.com/index/powering-product-discovery-in-chatgpt/) — ACP extended to **product discovery**: visual browsing, side-by-side comparison (price, reviews, features), image-upload inspiration search. Feed delivery via third parties including **Salesforce** and **Stripe**. Roadmap: personalization, local availability, ETAs
- [ChatGPT Merchants](https://chatgpt.com/merchants) — Merchant onboarding entry point for ACP discovery integration

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

### Agentic Commerce Trust Protocol (Alipay)

> **Note:** Distinct from Ant International's AMP above. AMP targets cross-border mobile surfaces via Alipay+; the Agentic Commerce Trust Protocol is Alipay's **domestic China** protocol linking AI-native apps to merchant/service platforms, settled through **Alipay AI Pay**.

- [The Paypers: Alipay rolls out the Agentic Commerce Trust Protocol](https://thepaypers.com/payments/news/alipay-rolls-out-the-agentic-commerce-trust-protocol-in-china) — Launched Jan 2026 with **Qwen App** (Alibaba's consumer AI app) as first adopter, connected to **Taobao Instant Commerce**; one integration lets merchants link to multiple AI agents without per-agent API development
- [Business Wire: Alipay AI Pay exceeds 120M transactions in one week (Feb 2026)](https://www.businesswire.com/news/home/20260213770962/en/Alipay-AI-Payment-Exceeds-120-Million-Transactions-in-One-Week-as-Agentic-Commerce-Accelerates-in-China) — First large-scale agentic payment service to reach this volume ([FinTech Magazine](https://fintechmagazine.com/news/alipay-hits-120m-weekly-ai-agent-transactions) · [Retail Technology Innovation Hub](https://retailtechinnovationhub.com/home/2026/2/12/alipay-ai-pay-solution-exceeds-120m-transactions-as-agentic-commerce-accelerates-in-china))
- The agent handles selection, ordering, and payment inside the Alipay AI Pay interface — no app-switching. Users place food and beverage orders by chatting with Qwen App

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
- [Visa Agent Directory (verified agent + merchant registry)](https://www.visa.co.uk/about-visa/newsroom/press-releases.3457328.html) — Alongside TAP, Visa's **Agent Directory** lets merchants and agents each confirm the other is a verified, legitimate party; this TAP + Agent Directory pairing is what unlocked merchant participation in the July 2 Europe launch. Cleverbridge among the first to enable it ([Cleverbridge / Las Vegas Sun, Jul 2](https://lasvegassun.com/news/2026/jul/02/cleverbridge-among-the-first-to-enable-visas-trust/))
- [Visa × OpenAI: agent payments in ChatGPT (Jun 2026)](https://www.axios.com/2026/06/10/visa-chatgpt-agents-commerce) — Visa integrated its payment tools into OpenAI's agent system to enable tokenized agent checkout in ChatGPT
- [Visa: Live agentic commerce in Europe (Jul 2, 2026)](https://www.visa.co.uk/about-visa/newsroom/press-releases.3457328.html) — First live agentic transactions across European merchants (lastminute.com, Frasers, Cleverbridge, BrickDepot) with 30+ issuers, secured via Visa Intelligent Commerce + Visa Payment Passkeys (SCA-compliant); announced at Visa Payments Forum, Paris ([Payment Expert](https://paymentexpert.com/2026/07/02/visa-agentic-payments-merchants-eu/), [Worldline/ING/Visa](https://www.globenewswire.com/news-release/2026/07/02/3321259/0/en/WORLDLINE-Worldline-ING-and-Visa-complete-a-live-agentic-payment-transaction-in-Europe-Press-release.html))

#### Visa × Mastercard × Ant International — Know Your Agent (KYA) Interoperability

- [Ant International, Mastercard and Visa initiate collaboration on Know Your Agent interoperability (Sep 9, 2026)](https://www.businesswire.com/news/home/20260909003891/en/Ant-International-Mastercard-and-Visa-Initiate-Collaboration-on-Know-Your-Agent-Interoperability-to-Scale-Agentic-Commerce) — The three networks will work toward **common KYA principles** so an agent verified under one scheme (Visa **Trusted Agent Protocol**, Mastercard **Verifiable Intent**, Ant **AMP**) is recognised across card networks, wallet ecosystems, agent platforms, and marketplaces without duplicate onboarding. Statement of intent only — **no spec, governance body, or timeline yet** — but the first cross-network agent-identity alignment among the three largest rails ([PYMNTS](https://www.pymnts.com/cybersecurity/2026/visa-mastercard-team-with-ant-know-your-agent-framework); [CNBC](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html); [Forkast analysis](https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/))

#### Mastercard Agent Pay

- [Press Release (Sep 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/september/mastercard-unveils-new-tools-and-collaborations-to-power-smarter%2C-safer-agentic-commerce.html)
- [Initial Announcement (Apr 2025)](https://www.mastercard.com/us/en/news-and-trends/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai.html)
- [Agent Pay international expansion, incl. Hong Kong (2026)](https://www.americanbanker.com/payments/news/visa-mastercard-expand-agentic-ai-deployments) — Part of Mastercard's push toward an international agentic-commerce network
- [Agent Pay for Machines (AP4M) — launch (Jun 10, 2026)](https://www.mastercard.com/us/en/news-and-trends/press/2026/june/mastercard-launches-agent-pay-for-machines.html) — Network for high-frequency, low-value agent-to-agent ("machine") payments. Four sequential functions — credentialing, permissioning, transacting (across Mastercard card + account rails), and settling in fiat or stablecoin. Agent permissions/credentials are recorded on **public blockchains** (initially Polygon, Solana, Base) rather than a private database, and AP4M uses Mastercard's **Verifiable Intent** framework. 30+ launch partners incl. Adyen, Ant International, BVNK, Checkout.com, Cloudflare, Coinbase, Stripe, Tempo, OKX, RippleX, Aave Labs. Interoperates with x402/MPP. ([Fortune](https://fortune.com/2026/06/10/mastercard-ai-payments-protocol-launch-agentic-finance/), [CoinDesk](https://www.coindesk.com/business/2026/06/10/mastercard-prepares-for-a-future-where-ai-agents-make-payments-with-latest-introduction))
- [Proto — agentic AI sandbox, live in UK (Aug 2026)](https://www.finextra.com/newsarticle/48097/mastercard-picks-uk-as-test-environment-for-agentic-ai-sandbox) — Mastercard's sandbox for retailers and FIs to test agent discoverability, trusted payment flows, and dispute handling before launch; announced Jul 16, live in the UK in August, with three new enterprise agents (shopping, onboarding, disputes) ([Payment Expert](https://paymentexpert.com/2026/07/16/mastercard-ai-sandbox-uk-payments/))

### Identity / Interop

- [Model Context Protocol (MCP) — Spec & Docs](https://modelcontextprotocol.io/) — Standard for AI agent tool interoperability
- [MCP Specification (GitHub)](https://github.com/modelcontextprotocol/specification) — Protocol spec repository
- [MCP Registry (Preview)](https://github.com/mcp) — GitHub MCP Registry for discovering MCP servers
- [WebMCP — Chrome origin trial](https://developer.chrome.com/blog/ai-webmcp-origin-trial) — Proposed web standard letting sites expose JavaScript functions and annotated HTML form elements as structured **tools** for in-browser AI agents. Moved from behind-a-flag prototype into a public **origin trial in Chrome 149** (docs May 18, 2026); early testers include Booking.com, Expedia, Shopify, Etsy, Instacart, and Target. Complements the payment/identity rails by standardizing how agents actuate merchant pages. ([InfoQ](https://www.infoq.com/news/2026/06/webmcp-web-agent-standard-chrome/))
- [**Web Bot Auth — IETF Working Group (`webbotauth`)**](https://datatracker.ietf.org/wg/webbotauth/about/) — Web Bot Auth is now a **chartered IETF working group** (Web and Internet Transport area; `charter-ietf-webbotauth-01` approved), not a set of individual drafts. Chairs David Schinazi and Rifaat Shekh-Yusef; AD Mike Bishop. Milestones: standards-track authentication and bot-information specs to the IESG Apr 2026, BCP operational spec Aug 2026. **Scope boundary worth noting:** the charter covers AI agents retrieving or interacting with content on behalf of end users, but explicitly places **agent-to-agent interfaces and end-user authentication out of scope** — that is the dividing line between Web Bot Auth and the AP2 / TAP / Agent Pay mandate layer
- [**HTTP Message Signatures for automated traffic — WG draft**](https://datatracker.ietf.org/doc/draft-ietf-webbotauth-httpsig-protocol/) — **`draft-ietf-webbotauth-httpsig-protocol-00`, adopted as a working-group document on Sep 1, 2026** (from `draft-meunier-webbotauth-httpsig-protocol-02`). This is now the canonical protocol document and the only active WG draft; it in turn replaces the expired `draft-meunier-web-bot-auth-architecture`
- [HTTP Message Signatures Directory](https://datatracker.ietf.org/doc/draft-meunier-webbotauth-httpsig-directory/) — Current directory draft (`draft-meunier-webbotauth-httpsig-directory`, Jun 26, 2026); **replaces** `draft-meunier-http-message-signatures-directory`
- [Registry and Signature Agent Card](https://datatracker.ietf.org/doc/draft-meunier-webbotauth-registry/) — Registry plus signature agent card format (`-03`, Jun 26, 2026)
- [Anonymous Bot Authentication](https://datatracker.ietf.org/doc/draft-rescorla-anonymous-webbotauth/) — Authorization and rate limiting for web agents without identifying the operator (Rescorla, `-01`, Jul 19, 2026)
- [Hosted Key Directories for Web Bot Auth](https://datatracker.ietf.org/doc/draft-singh-webbotauth-hosted-directories/) — Delegated key hosting for operators that cannot publish their own directory (Jul 19, 2026)
- [Web Bot Auth (Cloudflare Developer Docs)](https://developers.cloudflare.com/bots/reference/bot-verification/web-bot-auth/)
- [ZKProofport](https://zkproofport.app) — Zero-knowledge proof generation for AI agent identity. Lets agents prove Coinbase KYC, Country, Google OIDC, Google Workspace, or Microsoft 365 affiliation via x402-paid TEE proving on Base. ERC-8004 registered, A2A compatible. NPM: `@zkproofport-ai/mcp`. Reference app: [OpenStoa](https://github.com/zkproofport/openstoa) (1st place — The Synthesis Hackathon 2026)

### Accountability & Evidence Layer

> **Why this section exists:** every protocol above settles a transaction; none of them *adjudicate* one. x402, MPP, ACP, UCP and AP2 all presuppose a determination of whether the agent actually did what it was delegated to do — and none produce it. Three independent 2026 efforts converge on that gap from different directions: evidence (AEP), legal terms and dispute procedure (LCP), and clearing theory (RAILS).

#### A-Comm Evidence Protocol (AEP)

- [A-Comm](https://a-comm.ai/) — Open-source (Apache 2.0) evidence standard for agentic commerce. Every step — discovery, referral, intent, delegation, policy, cart, authorization, fulfillment — becomes an evidence artifact in a **tamper-evident hash chain sealed at authorization**, yielding an adjudication-ready record with observability, traceability, and auditability. Positioned explicitly as a *witness*: it wraps the protocols already in use without assigning weight, outcome, or liability, and charges no fees
- [Public comment open through Aug 14, 2026](https://www.prnewswire.com/news-releases/a-comm-technologies-inc-opens-public-comment-on-evidence-standard-for-agentic-commerce-302829047.html) — Draft opened for comment Jul 13, 2026 ([Digital Transactions](https://www.digitaltransactions.net/a-comms-agentic-prep-and-other-digital-transactions-news-briefs-from-7-20-26/))

#### Legal Context Protocol (LCP)

- [legalcontextprotocol.org](https://legalcontextprotocol.org/) — Open standard attaching **verifiable legal terms, consent, and dispute-resolution procedure** to transactions carried out by autonomous agents, so an agent can access and verify the terms governing a transaction it is about to execute. Specification, reference implementation, and companion white paper published
- [AAA press release (Jun 24, 2026)](https://www.adr.org/press-releases/aaa-and-industry-leaders-launch-legal-protocol-for-agentic-commerce/) — Stewarded by the **American Arbitration Association** and **Integra Ledger**. Founding contributors include Google, IBM, Circle, Wayfair, Stellar Development Foundation, Ava Labs, UiPath, Cardano, Hedera, Crossmint, Pinata, Aptos Foundation, Baselayer, Trinsic, First Person Cooperative, Sei Labs, and Mysten Labs ([overview](https://www.adr.org/news-and-insights/introducing-the-legal-context-protocol/), [Law.com](https://www.law.com/legaltechnews/2026/06/24/aaa-and-integra-ledger-announce-legal-protocol-for-ai-agent-transactions-/))

#### RAILS (research)

- [RAILS: Verification-Native Clearing for Agentic Commerce](https://arxiv.org/abs/2606.08790) — Academic framing of the same gap: argues **clearing is the missing primitive** and that the existing protocol stack assumes a determination none of it generates. See [Research Papers](#research-papers) for detail

> **Relationship to ERC-8183:** ERC-8183 solves adjudication *on-chain and in-contract* for agent-to-agent service delivery, with a designated Evaluator and escrowed funds. AEP, LCP and RAILS are protocol-agnostic and operate alongside card rails, stablecoin rails, and conversational checkout alike — evidence and legal context rather than escrow.

---

## 📄 Specifications & Whitepapers

### x402 Protocol

- [x402 Whitepaper (PDF)](https://www.x402.org/x402-whitepaper.pdf)
- [x402 Spec & Reference (GitHub)](https://github.com/coinbase/x402)

### A2A & AP2

- [A2A v1.0 Specification](https://a2a-protocol.org/latest/specification/)
- [AP2 Specification](https://ap2-protocol.org/specification/)
- [UCP Specification](https://ucp.dev/latest/specification/overview/) — Date-versioned snapshots; current is **v2026-08-25** ([release notes](https://github.com/Universal-Commerce-Protocol/ucp/releases/tag/v2026-08-25))

### ACP

- [ACP Spec (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) — Versioned snapshots (2025-09-29 through **2026-04-17**); current stable `2026-04-17`

### MPP

- [MPP Overview & Spec](https://mpp.dev/overview) — Protocol specification and payment flow documentation
- [IETF Payment HTTP Authentication Scheme](https://mpp.dev/overview) — See spec link on mpp.dev

### ERC-8183 / ERC-8004

- [ERC-8183 — Agentic Commerce](https://eips.ethereum.org/EIPS/eip-8183) — On-chain escrow standard for agent-to-agent service delivery (lifecycle, fee splits, evaluator role, expiry refund)
- [ERC-8004 — Trustless Agents](https://eips.ethereum.org/EIPS/eip-8004) — On-chain identity and reputation registries for autonomous agents (signed feedback, scoring rules hash, ERC-1271 contract signatures)

### Web Bot Auth / Agent Identity

- [IETF Working Group — Web Bot Auth (`webbotauth`)](https://datatracker.ietf.org/wg/webbotauth/about/) — Charter, milestones, and personnel
- [WG document list](https://datatracker.ietf.org/wg/webbotauth/documents/) — All related Internet-Drafts and RFCs
- [draft-ietf-webbotauth-httpsig-protocol](https://datatracker.ietf.org/doc/draft-ietf-webbotauth-httpsig-protocol/) — HTTP Message Signatures for automated traffic (**WG document**, adopted Sep 1, 2026; supersedes `draft-meunier-webbotauth-httpsig-protocol`)
- [draft-meunier-webbotauth-httpsig-directory](https://datatracker.ietf.org/doc/draft-meunier-webbotauth-httpsig-directory/) — HTTP Message Signatures Directory
- [draft-meunier-webbotauth-registry](https://datatracker.ietf.org/doc/draft-meunier-webbotauth-registry/) — Registry and Signature Agent card
- [draft-nottingham-webbotauth-use-cases](https://datatracker.ietf.org/doc/draft-nottingham-webbotauth-use-cases/) — Use cases for authentication of web bots
- [draft-rescorla-anonymous-webbotauth](https://datatracker.ietf.org/doc/draft-rescorla-anonymous-webbotauth/) — Anonymous bot authentication, authorization, and rate limiting

> **Naming note:** the protocol draft became a WG document (`draft-ietf-webbotauth-httpsig-protocol`) on Sep 1, 2026; the directory and registry drafts remain individual submissions for now. Earlier, the work was renamed under the `webbotauth` scheme in June 2026. The older `draft-meunier-web-bot-auth-architecture` is expired and archived, and `draft-meunier-web-bot-auth-directory` never existed as a Datatracker document — the directory work lived at `draft-meunier-http-message-signatures-directory` before being replaced. Cite the current drafts above.

> **Why it matters (Sep 2026):** Amazon began blocking **Meta's Muse** personal agent on Sep 20–21, citing no advance notice, **no agent self-identification** while browsing, and credential-capture concerns — the first high-profile retailer-vs-agent dispute over agent identity, and a live use case for Web Bot Auth, Visa TAP, and UCP agent identification ([GeekWire](https://www.geekwire.com/2026/amazon-blocks-metas-muse-ai-assistant-in-new-standoff-over-agentic-shopping/), [Retail Dive](https://www.retaildive.com/news/amazon-meta-muse-ai-agent-shopping-experience/831018/)). See [News](#meta-launches-muse-amazon-blocks-it-september-2026).

### Research Papers

- [RAILS: Verification-Native Clearing for Agentic Commerce](https://arxiv.org/abs/2606.08790) — de Valois-Franklin & Bogdan (Jun 7, 2026). Formalizes the **agentic clearing problem** — MCP, A2A, x402, AP2 and the network protocols each *assume* a determination of whether an agent met its delegated obligation, but none produce one. Proposes seven primitives (Obligation Object, Evidence Envelope, Verification Mesh, Clearing Decision, Settlement Instruction, Clearing Passport, Finality Rules) with a soundness property: no financially material settlement rests on evidence below the obligation's admissibility floor
- [Paying to Know: Micro-Transaction Markets for Verified Product Information in Agentic E-Commerce](https://arxiv.org/html/2606.24783) — Micro-transaction markets in which agents pay for verified product attributes rather than trusting merchant-supplied feeds
- "Towards Multi-Agent Economies: A2A + x402 Micropayments" — Proposes ledger-anchored identities with x402 for A2A micropayments

---

## 🛠 Developer Tools & Starters

### UCP Implementation

- [UCP GitHub Repository](https://github.com/Universal-Commerce-Protocol/ucp) — Spec, SDKs (Python, JavaScript), and reference implementations
- [UCP Python Sample](https://github.com/Universal-Commerce-Protocol/ucp) — See `samples/` in the repo
- [Google Merchant UCP Integration Guide](https://developers.google.com/merchant/ucp)
- [Anthropic — Claude Commerce Agents (`anthropics/commerce-agents`)](https://github.com/anthropics/commerce-agents) — Apache-2.0 reference blueprint (Sep 2, 2026): a customer-facing **shopping agent** (search, compare, cart, hand-off to the merchant's own checkout) and a staff-facing **merchant agent** (every write staged for human approval), with retail, travel, telecom, and entertainment examples; runs on the Messages API, Agent SDK, or Managed Agents, and ships a Claude Code scaffolding plugin. Protocol-agnostic — never places orders or charges cards itself
- [Shopify — Claude for Commerce examples](https://github.com/Shopify/claude-for-commerce-examples) — Shopify implementation of the blueprint: a storefront shopping agent over **UCP** endpoints with optional **Sign in with Shop**, handing off to the store's hosted checkout via `continue_url`; plus a merchant agent over the Admin API

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
- [Coinbase for Agents](https://www.coinbase.com/blog/coinbase-for-agents) — MCP server connecting external agents (ChatGPT, Claude) to a Coinbase account; uses **x402** to pay for premium research APIs and on-demand compute with no login/subscription. Agents run in a ring-fenced sub-portfolio with user-defined capital/asset limits. Launched Jun 11, 2026. ([TechCrunch](https://techcrunch.com/2026/06/11/coinbase-debuts-mcp-for-agent-trading/))
- [Ripple XRPL AI Starter Kit](https://ripple.com/insights/xrpl-ai-starter-kit/) — Developer kit for agentic payments on the XRP Ledger via **x402**, settling in XRP and **RLUSD**. First-phase release ships an XRPL Docs MCP server, two Claude skills (wallet + payment ops), and x402 integration; 3–5s settlement with fixed fees. Named a settlement partner in Mastercard AP4M. Launched Jun 10, 2026. ([PYMNTS](https://www.pymnts.com/blockchain/2026/ripple-targets-agentic-payments-market-with-xrpl-starter-kit/))
- [Glassnode agentic data access](https://research.glassnode.com/agentic-payments-glassnode-data-for-your-ai-agent/) — Pay-per-call access to on-chain metrics via **x402** in USDC — no API keys, subscriptions, or signup; MCP-capable agents discover an endpoint's price, pay, and retrieve data autonomously (Aug 2026)

#### SDKs & Libraries

- [x402 Monorepo (GitHub)](https://github.com/coinbase/x402) — `@x402/core`, `@x402/evm`, `@x402/svm`, `@x402/axios`, `@x402/fetch`, `@x402/express`, `@x402/hono`, `@x402/next`, `@x402/paywall`
- [x402 Rust crates + Facilitator](https://github.com/x402-rs/x402-rs)
- [x402-proxy](https://github.com/cascade-protocol/x402-proxy) — `curl` for x402 paid APIs. Auto-pays HTTP 402 responses with USDC, with MCP stdio proxy for AI agents

### ACP Implementation

- [ACP: Get Started (OpenAI)](https://developers.openai.com/commerce/guides/get-started/)
- [ACP Spec & Examples (GitHub)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol)
- [Stripe: Integrate the ACP](https://docs.stripe.com/agentic-commerce/protocol)

### MPP Implementation

- [MPP SDKs](https://mpp.dev/overview) — Official TypeScript SDK (`mppx`) with middleware for Hono, Express, Next.js, Elysia; Go, Ruby, Rust, and Python SDKs also published
- [Stripe: Machine Payments with MPP](https://docs.stripe.com/payments/machine/mpp) — Implementation with PaymentIntents
- [Visa Card Spec & SDK for MPP](https://corporate.visa.com/en/sites/visa-perspectives/innovation/visa-card-specification-sdk-for-machine-payments-protocol.html) — Card-based MPP transactions via tokenized network payment tokens settling over existing card infrastructure
- [MPP relays (Aug 3, 2026)](https://mpp.dev/blog/relays) — Delegate MPP payment validation and settlement without changing the application's payment flow
- [mppx identity support (Aug 12, 2026)](https://mpp.dev/blog/mppx-identity-support) — Verify agent identity across HTTP requests and payment retries
- [mppx for agent SDKs and harnesses (Jul 27, 2026)](https://mpp.dev/blog/mppx-agent-runtimes) — Hooks connecting agent runtimes to paid tools and HTTP services through MPP; mpp.dev now lists **Amazon, Alchemy, Browserbase, Cloudflare, Dune, Parallel, and Visa** as integrations

### A2A Implementation

- [A2A Samples Repository](https://github.com/a2aproject/a2a-samples) — Hello-world, multi-agent, and framework-specific examples
- [A2A Inspector](https://github.com/a2aproject/a2a-inspector) — Validate your A2A agent

### ERC-8183 / ERC-8004 Implementation

- [CardZero](https://cardzero.ai) — First known production deployment of ERC-8004 + ERC-8183 on Base mainnet. ERC-4337 smart-contract wallet for AI agents with owner-set spending rules, x402 buyer support, and full Job-escrow lifecycle live at `api.cardzero.ai/v1/jobs`. Source on [GitHub](https://github.com/mrocker/CardZero); MCP server published as [`cardzero-mcp`](https://www.npmjs.com/package/cardzero-mcp); 27-page docs + `/llms-full.txt` corpus at [cardzero.ai/docs](https://cardzero.ai/docs).

### Agent Frameworks & Managed Platforms

#### Amazon Bedrock AgentCore Payments

- [AWS What's New: AgentCore Payments — generally available (Aug 18, 2026)](https://aws.amazon.com/about-aws/whats-new/2026/08/bedrock-agentcore-payments-ga/) — Managed surface for agents to pay for APIs, MCP servers, web content, and other agents; **GA** adds **MPP support** and the **x402 "upto"** spending-ceiling scheme
- [AWS ML Blog: AgentCore payments GA deep dive](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale/) — Coinbase and Stripe Privy wallet integrations, protocol orchestration across x402 and MPP, configurable infrastructure-level payment limits, transaction observability
- [AWS ML Blog: Agents that transact (preview announcement, built with Coinbase and Stripe)](https://aws.amazon.com/blogs/machine-learning/agents-that-transact-introducing-amazon-bedrock-agentcore-payments-built-with-coinbase-and-stripe/) — Wraps x402 negotiation, wallet auth, stablecoin settlement, and proof delivery; deterministic session spending limits at the infra layer
- [Coinbase Blog: AgentCore Payments powered by x402](https://www.coinbase.com/blog/introducing-amazon-bedrock-agentcore-payments-powered-by-x402-and-coinbase)
- [Sample: AgentCore + CloudFront + x402](https://github.com/aws-samples/sample-agentcore-cloudfront-x402-payments) — Reference demo using Bedrock AgentCore, Strands SDK, and CloudFront
- [Tutorial 09: Pay per use with the x402 `upto` scheme](https://github.com/awslabs/agentcore-samples/tree/main/01-features/08-agents-that-transact/00-getting-started/09-pay-per-use-with-upto) — Runnable **`upto`** reference implementation: a Strands agent buys metered inference on Base mainnet, authorizing a **ceiling** while the seller settles actual consumption via **Permit2** (one-time `approve` per wallet, gas in ETH). Includes a fail-closed `UptoOnlyPaymentHandler` for pinning the scheme when a seller advertises both `exact` and `upto`; requires `bedrock-agentcore>=1.22.0`
- [Tutorial 08: MPP (Machine Payments Protocol)](https://github.com/awslabs/agentcore-samples/tree/main/01-features/08-agents-that-transact/00-getting-started/08-mpp-machine-payments-protocol) — MPP counterpart tutorial on the Tempo Moderato testnet (chain 42431); contrasts MPP `charge`/`session` intents with x402 `exact`/`upto` schemes from the same AgentCore payments surface
- [Use case: Pay for Secure Data (x402)](https://github.com/awslabs/agentcore-samples/tree/main/01-features/08-agents-that-transact/02-use-cases/pay-for-x402-secure-data) — **"Trust before spend"** pattern: before paying a target x402 service (Heurist YahooFinanceAgent), the agent first pays **t54 x402-secure** to risk-score that exact endpoint; a deterministic, fail-closed `TrustedX402ServiceGateway` blocks the target payment in code (not by prompt) on missing/stale/low-score/scam-flagged trust results. Four-role IAM separation (session creation vs payment signing), per-session spend caps, agent never holds private keys

#### Cloudflare Agents SDK

- [Agents SDK Overview](https://developers.cloudflare.com/agents/)
- [x402 in Agents SDK](https://developers.cloudflare.com/agents/x402/) — Built-in x402 support
- [MPP in Agents SDK](https://developers.cloudflare.com/agents/agentic-payments/mpp/) — Built-in MPP support
- [Cloudflare Blog: x402 Foundation](https://blog.cloudflare.com/x402/)

#### Cloudflare Monetization Gateway

- [Cloudflare Blog: Announcing the Monetization Gateway](https://blog.cloudflare.com/monetization-gateway/) — **Sell-side** x402 product (announced Jul 1, 2026; **waitlist only**) letting Cloudflare customers charge any caller for any protected resource — web pages, datasets, APIs, or **MCP tools** — with **stablecoin settlement over x402** enforced at the edge (330+ cities). Sellers write payment rules as WAF-style expressions (per-verb pricing, variable pricing, intercept origin `401`→`402`), managed via dashboard, API, or Terraform; buyers need no signup/API key (optional **Web Bot Auth** agent identity). Settles in USDC (Base) and Open USD — sub-second, sub-cent, no chargebacks. Generalizes Cloudflare's earlier [Pay Per Crawl](https://blog.cloudflare.com/introducing-pay-per-crawl/) (charging AI crawlers) to any caller/resource. ([InfoQ](https://www.infoq.com/news/2026/07/cloudflare-aws-x402-micropayment/), [crypto.news](https://crypto.news/cloudflare-opens-waitlist-for-x402-stablecoin-monetization-gateway/))

#### Cloudflare Agent Wallets & Agents Week (Aug 2026)

- [Cloudflare: programmable wallets for AI agents](https://blog.cloudflare.com/wallets/) — Provision stablecoin-backed wallets per account and virtual wallets per agent, with spending allowances, transaction limits, and merchant restrictions; x402-compatible payments paired with delegated identity
- [WebMCP developer preview](https://blog.cloudflare.com/webmcp/) — Expose structured browser-agent actions from ordinary websites without a separate API
- [Agent Readiness & Answer Engine Optimization](https://blog.cloudflare.com/aeo/) — Measure whether agents can discover/interpret a site and how often AI assistants recommend it
- [WriteGuard (private beta)](https://blog.cloudflare.com/mcp-portal-writeguard-private-beta/) — Least-privilege authorization for MCP write operations (purchase, refund, account changes)
- [The Agent Access Model](https://blog.cloudflare.com/the-agent-access-model/) — Task-scoped delegated authority: identity brokering + continuous mediation + stateful trust

#### Adyen Agentic

- [Adyen Agentic (press)](https://www.adyen.com/press-and-media/adyen-agentic) — Protocol-agnostic, three-layer API suite for agentic commerce: **Agentic Feed** (real-time catalog/pricing/availability), **Agentic Cart** (orchestrates checkout, tax, fulfillment, order management), and **Agentic Payments** (auth, token portability, merchant-of-record preservation, fraud/risk). Launched Jun 16, 2026 in limited US availability. Strategic partners incl. American Express, Mastercard, Salesforce, Visa. ([PYMNTS](https://www.pymnts.com/news/b2b-payments/2026/adyen-debuts-agentic-solutions-for-enterprise-merchants/))

#### Nuvei Agentic

- [Nuvei Agentic (press)](https://www.nuvei.com/posts/nuvei-completes-first-party-in-agent-payment-with-visa-unveils-merchant-led-agentic-payments-strategy) — Merchant-led, protocol-agnostic agentic payments strategy built on two components: a **Protocol Compatibility Layer** (integrate once, accept payments from whichever standard an agent uses — **ACP, AP2, or MCP** — routed across networks) and **Know Your Agent (KYA)** (registers/credentials agents, validates the consumer's mandate, scores agent reputation, keeps actions auditable). Announced alongside Nuvei's first-party **in-agent** payment on live **Visa** rails (with Arvato Systems and brand Kings and Priests), settled via Visa Intelligent Commerce under shopper-set guardrails (spend caps, approved categories). Initial availability targeted for H2 2026 (protocol compatibility, KYA registry + risk scoring, network certifications, developer sandbox). Announced Jul 2, 2026. ([The Paypers](https://thepaypers.com/payments/news/nuvei-completes-its-first-in-agent-payment-on-visa-rails), [PR Newswire](https://www.prnewswire.com/news-releases/nuvei-completes-first-party-in-agent-payment-with-visa-unveils-merchant-led-agentic-payments-strategy-302816873.html))

#### MCP Integration

- [OpenAI Agents SDK — MCP](https://openai.github.io/openai-agents-python/mcp/)
- [Stripe MCP Server](https://docs.stripe.com/) — Stripe's MCP tools for agentic commerce

---

## 🌐 Ecosystem & Partners

### UCP

Co-developed by **Google** and **Shopify**. Endorsed by 20+ partners including Etsy, Wayfair, Target, Walmart, Adyen, American Express, Best Buy, Flipkart, Macy's Inc., Mastercard, Stripe, The Home Depot, Visa, and Zalando. ([Source: Google Blog, Jan 2026](https://blog.google/products/ads-commerce/agentic-commerce-ai-tools-protocol-retailers-platforms/)). May 2026: **Universal Cart** extends the cart across **Search, Gemini, YouTube, and Gmail**, built on Google Wallet, with UCP-powered checkout via Google Pay — live merchants include **Nike, Sephora, Target, Ulta Beauty, Walmart, Wayfair**, and Shopify merchants such as **Fenty** and **Steve Madden**; the brand always remains merchant of record. Rolling out across Search and the Gemini app in the U.S. over summer 2026, YouTube and Gmail to follow. UCP checkout expands to **Canada and Australia** in the coming months and the **U.K.** later, with new verticals starting in **hotel booking and local food delivery**. ([Source: Google I/O 2026](https://blog.google/products-and-platforms/products/shopping/google-shopping-cart/); [Google Marketing Live](https://blog.google/products-and-platforms/products/shopping/shopping-updates-google-marketing-live/)) June 2026: Shopify made UCP **self-serve** — from Jun 17, any developer can register an agent profile in the Shopify Developer Dashboard and call the public MCP endpoint with no approval gate. ([Source: Shopify](https://www.shopify.com/news/ai-commerce-at-scale)) August–September 2026: the **v2026-08-25** spec shipped (3DS2, Web Bot Auth interop, multi-vertical refactor, grocery, payment schedules), and the **Payments Technical Council** was seated on Sep 2 with Adyen, Ant International, Coinbase, Global Payments, Google, PayPal, Shopify, and Stripe — notably placing a stablecoin-native member (Coinbase) and Ant alongside the card-side PSPs on UCP's payment-layer governance. ([Source: ucp.dev](http://ucp.dev/documentation/announcements/)) Mid/late September 2026: Shopify enabled **identity linking** fleet-wide (7,355 stores declaring it by Sep 19), **Wix** began rolling out **cart** (Sep 22), UCP stores now span **14** commerce platforms (incl. Salla, Zid, Boutir, Cafe24, Tiendanube, Jumpseller, BigCommerce), and **Salesforce Commerce Cloud** set UCP GA for **October 2026**. ([Source: UCP Checker](https://ucpchecker.com/blog/state-of-agentic-commerce-september-2026); [Salesforce](https://www.salesforce.com/commerce/ai/agentic-commerce/universal-commerce-protocol/))

### AP2

In April–May 2026 Google **donated AP2 to the FIDO Alliance** for open, community-led governance, alongside the **v0.2** release. FIDO stood up two working groups — Agentic Authentication (chaired by CVS Health, Google, OpenAI) and Payments (chaired by Mastercard and Visa) — developing interoperable standards based on AP2 and Mastercard's Verifiable Intent. Officially reported supporters include Shopify, Etsy, Salesforce, Mastercard, PayPal, American Express, Adyen, Worldpay, and 60+ partners total. ([Source: Google Blog](https://blog.google/products-and-platforms/platforms/google-pay/agent-payments-protocol-fido-alliance/); [AP2 Protocol site](https://ap2-protocol.org/))

### x402 Foundation

x402 is governed by the **x402 Foundation under the Linux Foundation**. The Foundation was announced in **April 2026** (founding contributors Coinbase, Cloudflare, and Stripe) and reached **operational launch on July 14, 2026**, with Coinbase's contribution of the protocol completed and **40 members** seated across two tiers:

- **Premier (17):** Adyen, AWS, American Express, Circle, Cloudflare, Coinbase, Fiserv, Google, Mastercard, Monad Foundation, MoonPay, Ripple, Shopify, Solana Foundation, Stellar Development Foundation, Stripe, Visa
- **General:** Aleo, Fireblocks, Galaxia Moneytree, Hecto Financial, Injective, KakaoPay, Kite AI, LayerZero Labs, Merit Systems, NEAR Foundation, Orthogonal, Polygon Labs, Quant Network, SKALE, t54 labs, utexo, World Liberty Financial, zerohash

Notably, **Visa and Mastercard both sit as premier members** of a stablecoin-native standard while simultaneously running their own agent trust rails (TAP / Agent Pay) and co-chairing the FIDO Payments working group on AP2 — the card networks are hedging across all three governance tracks. ([Source: Linux Foundation, Jul 2026](https://www.linuxfoundation.org/press/linux-foundation-announces-operational-launch-of-x402-foundation-to-standardize-internet-native-payments-for-ai-agents-and-applications); [PYMNTS](https://www.pymnts.com/news/2026/40-finance-and-tech-giants-unite-to-standardize-agentic-payments/))

The Cloudflare Agents SDK and MCP servers support x402 out of the box. x402 v2 adds modular payment scheme support for EVM and Solana networks. As of mid-2026, **AWS Bedrock AgentCore** also wraps x402 as a managed payment surface (built with Coinbase and Stripe), and the **Coinbase x402 Bazaar** exposes 10,000+ payable endpoints. Per Chainalysis, x402 passed **100M agentic transactions on Base** in Q1 2026 and reached ~169M cumulative by July 2026 (Base added ~20M transfers in a recent 90-day window; ~95% of agentic payment *value* now flows in transactions above $1); Coinbase separately reported x402 processed ~75M transactions and ~$24M volume in a trailing 30-day window as of June 2026. Per Coinbase's **AiFi** announcement (Aug 27, 2026), x402 has now passed **205M cumulative agent transactions (~$53M volume)**, with ~14M transfers in the trailing 30 days (Base 7.3M, Polygon 5.6M) settled almost entirely in USDC. ([Coinbase](https://x.com/coinbase/article/2092995079640141855); [GNCrypto](https://www.gncrypto.news/news/coinbase-x402-14m-ai-agent-payments-usdc-base-polygon/)) In July 2026 Cloudflare announced the **Monetization Gateway** (waitlist), a sell-side product that charges callers for pages, APIs, datasets, and MCP tools with x402 stablecoin settlement enforced at the edge.

### ACP

**OpenAI + Stripe** co-developed ACP. The consumer-facing **Instant Checkout** experience in ChatGPT was **discontinued in early 2026** after a ~5-month trial (low adoption, weak conversion, unresolved sales-tax handling). ACP did not shrink so much as **change shape**: OpenAI extended it into a **discovery-and-handoff layer**, with merchants sharing product feeds and promotions into ChatGPT and shoppers routed to the merchant's own checkout. Seven major retailers are integrated for discovery — **Target, Sephora, Nordstrom, Lowe's, Best Buy, The Home Depot, and Wayfair** — and **all Shopify merchants** are included automatically via **Shopify Catalog** with no per-merchant work. Feeds can be delivered through third parties including **Salesforce** and **Stripe**. Merchants wanting deeper integration build **ChatGPT apps**: **Walmart** shipped an in-ChatGPT experience with account linking, loyalty, and native Walmart payments (web live, iOS/Android to follow). ACP remains open to any PSP — Stripe provides the first implementation via Shared Payment Token, with PayPal also involved. ([Source: OpenAI, Mar 2026](https://openai.com/index/powering-product-discovery-in-chatgpt/); [TechCrunch](https://techcrunch.com/2026/03/24/openais-plans-to-make-chatgpt-more-like-amazon-arent-going-so-well/))

### MPP / Tempo

**Stripe + Tempo Labs (Paradigm)** co-authored MPP. Design partners include Anthropic, DoorDash, Mastercard, Nubank, OpenAI, Ramp, Revolut, Shopify, Standard Chartered, and Visa. Cloudflare supports MPP in its Agents SDK. ([Source: Stripe Blog, Mar 2026](https://stripe.com/blog/machine-payments-protocol))

### AMP / Ant International

Open-sourced by **Ant International** and implemented with **Alipay+** wallet partners (40+ wallets, 1.8B accounts, 150M merchants). AMP targets mobile-native agentic payments across smartphones, smartwatches, AR glasses, and in-car systems. ([Source: Business Wire, Apr 2026](https://www.businesswire.com/news/home/20260427209524/en/Ant-International-Launches-Open-Sourced-Agentic-Mobile-Protocol-to-Drive-AI-Commerce))

### Agentic Commerce Trust Protocol / Alipay (China)

**Alipay** launched the **Agentic Commerce Trust Protocol** in January 2026 as a common integration layer between AI-native apps and merchant/service platforms in China. **Qwen App** — Alibaba's consumer AI application — was the first adopter, connected to **Taobao Instant Commerce** and Alipay's AI payment service. Settlement runs through **Alipay AI Pay**, which exceeded **120 million transactions in a single week** as of February 2026, making it the first large-scale agentic payment service to reach that volume. For scale context, that weekly figure is comparable to x402's *cumulative* transaction count over the same period — the largest agentic payment deployment in production today is domestic Chinese. ([Source: Business Wire, Feb 2026](https://www.businesswire.com/news/home/20260213770962/en/Alipay-AI-Payment-Exceeds-120-Million-Transactions-in-One-Week-as-Agentic-Commerce-Accelerates-in-China); [The Paypers](https://thepaypers.com/payments/news/alipay-rolls-out-the-agentic-commerce-trust-protocol-in-china))

### Agent Trust Rails

**Visa's Trusted Agent Protocol** and **Mastercard's Agent Pay** both leverage **Web Bot Auth** for cryptographically signed agent identity during browse and payment flows. In 2026 both expanded internationally — Visa's Agentic Ready program to Latin America and Asia (reaching the first live agentic transactions with European merchants in July 2026), and Mastercard's Agent Pay to markets including Hong Kong. In June 2026 Mastercard also launched **Agent Pay for Machines (AP4M)**, a dedicated network for high-frequency agent-to-agent payments with on-chain agent credentialing (Polygon/Solana/Base) and Verifiable Intent. In August 2026, Mastercard's **Proto** agentic AI sandbox went live in the UK as its first test market, and both networks joined Rain's **Agentic Payments Alliance** (26 founding members incl. Visa, Mastercard, Circle, Fiserv, Fireblocks) working on shared agent identity, authorization, and fraud standards. In September 2026 Mastercard seated the inaugural 22-company **Start Path Agentic Commerce & Services** cohort, including **t54** (x402-secure / XRPL x402 facilitator with Verifiable Intent), Skyfire, Crossmint, Tunic Pay, and Nevermined. ([The Paypers](https://thepaypers.com/payments/news/mastercard-start-path-adds-22-firms-to-agentic-commerce-track)) On Sep 9, 2026 **Visa, Mastercard, and Ant International** announced a joint **Know Your Agent (KYA) interoperability** effort to align TAP, Verifiable Intent, and AMP under common trust principles — no spec or governance body yet. ([Business Wire](https://www.businesswire.com/news/home/20260909003891/en/Ant-International-Mastercard-and-Visa-Initiate-Collaboration-on-Know-Your-Agent-Interoperability-to-Scale-Agentic-Commerce))

### Agent Reputation & Scoring

- [DJD Agent Score](https://djd-agent-score.fly.dev) — Behavioral reputation scoring API for AI agent wallets on Base. Scores agents 0–100 across 5 dimensions using on-chain transaction patterns, sybil detection, and gaming velocity checks. x402-native monetization, MCP server distribution, and ERC-8004 compatible. ([GitHub](https://github.com/jacobsd32-cpu/djd-agent-score))
- **t54 x402-secure** — Paid x402 endpoint risk-scoring service (overall score, risk level, scam flag) from t54 labs (x402 Foundation member); featured as the trust guardrail in AWS's official [Pay for Secure Data use case](https://github.com/awslabs/agentcore-samples/tree/main/01-features/08-agents-that-transact/02-use-cases/pay-for-x402-secure-data), where an agent pays to vet an endpoint before paying the endpoint itself. Sep 2026: selected for **Mastercard Start Path's inaugural Agentic Commerce & Services cohort** (identity verification, risk assessment, dispute resolution for merchants/networks transacting with agents); also operates the **x402 facilitator on XRPL** with Ripple, integrating Mastercard **Verifiable Intent** ([The Paypers](https://thepaypers.com/payments/news/mastercard-start-path-adds-22-firms-to-agentic-commerce-track))

### Analytics & Dashboards

- [agenteconomy.to](https://agenteconomy.to) — Real-time dashboard tracking AI agent on-chain payment activity across x402, ERC-8004, ERC-8183 (Virtuals ACP), and MPP (Stripe/Tempo) on 8 chains. Aggregated event counter, chain distribution, facilitator share, and time-series charts. Data refreshes every 6 hours. ([source](https://github.com/realdora/agenteconomy))

### Payments Networks

- **Visa** — Trusted Agent Protocol; Agentic Ready program (expanded to LatAm & Asia 2026; first live agentic transactions in Europe, Jul 2026); card specification + SDK extending MPP to card payments (2026); Open USD consortium member
- **Mastercard** — Agent Pay (international expansion incl. Hong Kong, 2026); **Agent Pay for Machines (AP4M)** launched Jun 2026 for high-frequency machine-to-machine payments, with on-chain agent credentials (Polygon/Solana/Base) and Verifiable Intent, settling in fiat or stablecoin, 30+ partners; acquired BVNK for stablecoin infrastructure; **Proto** sandbox live in UK (Aug 2026); inaugural **Start Path Agentic Commerce** cohort of 22 startups incl. t54 (Sep 2026)
- **PayPal** — AP2 support; ACP participant; upcoming UCP payment method
- **American Express** — AP2 partner, UCP endorser
- **Adyen** — AP2 integration, UCP endorser; launched **Adyen Agentic** (Jun 2026), a three-layer, protocol-agnostic suite (Agentic Feed, Agentic Cart, Agentic Payments) for selling through AI agents
- **Worldpay** — AP2 support
- **Nuvei** — **Nuvei Agentic** (Jul 2026): merchant-led, protocol-agnostic execution layer (Protocol Compatibility Layer across ACP/AP2/MCP + Know Your Agent registry); completed a first-party in-agent payment on live Visa rails; general availability targeted H2 2026
- **Stripe** — ACP co-creator, MPP co-author, UCP endorser; agreed to acquire **OpenRouter** ($7B+, Aug 2026) to extend into the model-consumption/token-metering layer
- **NPCI / UPI (India)** — **Unified Agent Protocol** (in development; **not yet published or launched**): reported design lets registered/verified agents transact on UPI within user-set limits without per-transaction approval, built on UPI Circle delegation. At Global Fintech Fest 2026 (Sep 8–11) NPCI's chairman publicly acknowledged NPCI is "examining the protocols" for agent identification/authorisation but stressed AI "may recommend" while authentication and settlement stay deterministic; no spec or launch date was given ([MediaNama](https://www.medianama.com/2026/09/223-npci-ai-agents-upi-payments/); [Reuters](https://www.brecorder.com/news/40437409/india-preparing-rollout-of-agentic-payments-on-upi-sources-say))
- **AWS** — Bedrock AgentCore Payments (**GA Aug 2026**), managed x402 + MPP + Stripe surface built with Coinbase and Stripe
- **GoCardless** — Processed the **UK's first live agentic account-to-account payment** (announced Sep 22, 2026): an AI agent set up a Direct Debit mandate in-conversation for a recurring donation to Trussell, built under the FCA's AI Live Testing programme — an open-banking / bank-rail alternative to card and stablecoin agent payments

### Stablecoin & Settlement Infrastructure

- **Open USD (OUSD)** — Shared-governance, USD-backed stablecoin consortium unveiled Jun 30, 2026 by 140+ firms (Stripe, Visa, Mastercard, Coinbase, BlackRock, BNY, Google, Shopify, Fireblocks, Aave, Solana); fee-free mint/redeem with reserve income shared among members, going live on Solana, Stellar, Base, and Polygon later in 2026. Positioned as a neutral settlement layer / alternative to USDC & USDT for agent-driven payments ([Fortune](https://fortune.com/2026/06/30/stripe-visa-stablecoin-rival-ousd-tether-circle/), [CoinDesk](https://www.coindesk.com/business/2026/06/30/circle-slides-8-as-stripe-coinbase-and-blackrock-back-rival-stablecoin-network), [Forrester](https://www.forrester.com/blogs/stripes-new-stablecoin-bet-open-usd/))
- **AllUnity (SEKAU)** — Launched the first fully reserved, MiCA-compliant Swedish krona-backed stablecoin, SEKAU, on Jun 19, 2026, live on Ethereum, Solana, Base, Tempo, and Polygon (Banking Circle as reserve/transaction bank); settles AI-initiated transactions into local bank accounts, extending AllUnity's x402-powered agentic settlement layer ([AllUnity](https://allunity.com/news/allunity-launches-the-first-fully-reserved-swedish-krona-backed-stablecoin-sekau), [CoinDesk](https://www.coindesk.com/business/2026/05/20/germany-s-allunity-plans-swedish-krona-stablecoin-pushes-into-ai-agentic-payments))
- **Fireblocks** — Agentic Payments Suite for stablecoin transactions ([The Paypers](https://thepaypers.com/payments/news/fireblocks-launches-agentic-payments-suite-for-stablecoin-transactions))
- **Circle + Nium** — Partnership to strengthen stablecoin rails for agentic AI payments ([American Banker](https://www.americanbanker.com/payments/news/circle-and-nium-partner-to-boost-stablecoins-ai))
- **Natural** — Secured a credit facility of up to **$100M from Upper90** (Aug 2026), atop $40M equity, specifically to scale payments for AI agents — first dedicated credit capacity underwriting agent-payment float (funds often advanced before downstream settlement) ([Natural](https://www.natural.com/blog/100m-credit-facility))
- **Ripple (RLUSD)** — XRPL AI Starter Kit (Jun 2026) lets agents settle in RLUSD (Ripple's NYDFS-approved USD stablecoin) and XRP over x402 ([Ripple](https://ripple.com/insights/xrpl-ai-starter-kit/))

### AI / Agent Platforms

- **Google Cloud** — AP2 creator, UCP co-developer
- **OpenAI** — ACP co-creator (with Stripe)
- **Anthropic** — MPP design partner; released **Claude Commerce Agents** (Sep 2026), open-source shopping + merchant agent blueprints, with a Shopify UCP storefront implementation
- **Meta** — **Muse** personal agent (Sep 8, 2026) that shops and pays on users' behalf, including via browser automation; Shopify partnered for agentic checkout, while Amazon blocked it (Sep 20–21) over agent identification
- **Shopify** — UCP co-developer, AP2 & ACP partner
- **AWS** — Bedrock AgentCore Payments (x402 + MPP + Stripe; GA Aug 2026), with the x402 Bazaar MCP server via AgentCore Gateway

### Crypto & Web3

- **Coinbase** — x402 creator, AP2 partner, AgentCore Payments partner; **AiFi (Agentic Finance)** framing launched Aug 2026 with x402 at 205M cumulative transactions
- **Tempo Labs** — MPP co-author (Paradigm-backed, payments-optimized L1)
- **Radius Network** — x402-compatible stablecoin L1 for agentic micropayments (mainnet launched Mar 2026; sub-second finality, sub-penny fees) ([docs](https://docs.radiustech.xyz/developer-resources/x402-integration))
- **Ripple / XRPL** — XRPL AI Starter Kit (Jun 2026) for agentic payments via x402, settling in XRP and RLUSD; XRPL named a settlement partner in Mastercard AP4M ([Ripple](https://ripple.com/insights/xrpl-ai-starter-kit/)); XRPL agentic transactions reportedly neared **4M by Sep 5, 2026** with t54 operating the x402 facilitator ([The Currency Analytics](https://thecurrencyanalytics.com/altcoins/xrp-ledger-ai-transactions-near-4-million-as-t54-and-mastercard-back-agentic-commerce-290849))
- **Binance — Agent OS** — Standardized layer (launched Aug 2026) connecting external AI applications to Binance market data, wallets, payments, and on-chain functions; initial MCP implementation supports dedicated subaccounts, configurable permissions, and revocation — separating agent reasoning from tightly controlled execution authority ([PR Newswire](https://www.prnewswire.com/news-releases/binance-introduces-agent-os-to-connect-ai-applications-to-financial-infrastructure-302856306.html))
- **Circle — Arc L1 + Agent Stack** — [Agent Stack](https://www.circle.com/blog/introducing-circle-agent-stack-financial-infrastructure-for-the-agentic-economy) (launched May 11, 2026) gives agents controlled USDC access — Agent Wallets, Agent Marketplace, Circle CLI, Circle Skills, and **Nanopayments** (gas-free USDC transfers as small as one-millionth of a dollar via Circle Gateway). Settlement targets **Arc**, Circle's stablecoin-native L1 (USDC as native gas); Arc has run a public testnet since Oct 2025 with **mainnet expected summer 2026** (still pre-mainnet as of Jul 2026). Circle also raised a **$222M ARC token presale** (backers incl. BlackRock, a16z). ([Decrypt](https://decrypt.co/367490/circle-ai-agents-usdc-stablecoin-powers-222m-arc-token-sale), [Phemex](https://phemex.com/news/article/circle-unveils-arc-blockchain-whitepaper-mainnet-launch-set-for-summer-2026-82817))

---

## 📰 News & Analysis

### Major Launches & Milestones

#### Meta Launches Muse; Amazon Blocks It (September 2026)

- [TechCrunch: Meta debuts its Muse AI agent (Sep 8, 2026)](https://techcrunch.com/2026/09/08/meta-debuts-its-muse-ai-agent-will-consumers-trust-it/) — Personal agent that executes multi-step tasks across email, calendar, payments, dining, and shopping; free with paid tiers on iOS, Android, web, and WhatsApp; operates services without APIs through a browser. Rose to **#1 on the U.S. App Store**; Shopify announced a partnership enabling agentic checkout on Shopify stores
- [GeekWire: Amazon blocks Meta's Muse (Sep 2026)](https://www.geekwire.com/2026/amazon-blocks-metas-muse-ai-assistant-in-new-standoff-over-agentic-shopping/) — Amazon began blocking Muse on Sep 20–21, saying it was not notified, the agent **does not identify itself** when browsing, and it appears to capture customer credentials (Meta says Muse never sees passwords or payment details). The dispute is about **agent identity and terms of access**, not payment rails — the problem Web Bot Auth, TAP, KYA, and UCP agent identification aim to solve
- [Retail Dive](https://www.retaildive.com/news/amazon-meta-muse-ai-agent-shopping-experience/831018/) · [CNBC](https://www.cnbc.com/2026/09/21/meta-muse-personal-ai-agent-downloads.html) · [The Register](https://www.theregister.com/ai-and-ml/2026/09/21/amazon-shows-metas-muse-ai-shopping-agent-the-door/5297777)

#### UCP Adoption Surge — Shopify Identity Linking, Wix Cart, 14 Platforms (September 2026)

- [UCP Checker: State of Agentic Commerce — September 2026](https://ucpchecker.com/blog/state-of-agentic-commerce-september-2026) — Shopify moved its template to **v2026-08-25** on Aug 28–29 (~10,600 stores), then enabled **identity linking** on Sep 17–19 (27 → **7,355** stores, all delegating to Shop accounts); **Wix** began rolling out **cart** on Sep 22 (3,549 of 6,929 stores by mid-afternoon). Census: **17,767 verified stores**, **14** named platforms with a verified store (Salla, Zid, Boutir, Cafe24, Tiendanube, Tray, Jumpseller, BigCommerce, WooCommerce, and more), and the **first production merchant declaring a payment token**. Shopping TC minutes put the **next spec release in early December or January**
- Caveat: nearly all identity linking now runs through a **single provider** (Shop accounts), and payment tokens remain effectively pre-production

#### Salesforce Commerce Cloud Sets UCP GA for October 2026 (September 2026)

- [Salesforce: Universal Commerce Protocol](https://www.salesforce.com/commerce/ai/agentic-commerce/universal-commerce-protocol/) — Announced at Dreamforce (Sep 15): UCP integration for Commerce Cloud reaches **GA in October 2026**, enabling discovery and checkout in Google Search / AI Mode and Gemini while payments, compliance, and order management stay on the merchant's existing stack. Potentially the largest new-platform UCP event since Wix ([UCP Checker: what Commerce Cloud storefronts declare pre-launch](https://ucpchecker.com/blog/salesforce-commerce-cloud-ucp-october))

#### GoCardless — UK's First Live Agentic Account-to-Account Payment (September 2026)

- [GoCardless: first agentic A2A payment in the UK](https://gocardless.com/blog/gocardless-first-agentic-payment-uk) — An AI agent explained the charity Trussell's work, offered monthly donation tiers, and set up a **Direct Debit mandate** without the donor leaving the conversation. Built through the **FCA's AI Live Testing** programme; positions account-to-account (open banking) rails as a foundation for agentic payments alongside cards and stablecoins
- [Finextra](https://www.finextra.com/pressarticle/110969/gocardless-processes-first-agentic-account-to-account-transaction-in-the-uk) · [Open Banking Expo](https://www.openbankingexpo.com/news/gocardless-processes-the-first-agentic-account-to-account-payment-in-the-uk/) · [FinTech Global](https://fintech.global/2026/09/22/gocardless-completes-uks-first-agentic-bank-payment/)

#### Anthropic Open-Sources Claude Commerce Agents (September 2026)

- [GitHub: anthropics/commerce-agents](https://github.com/anthropics/commerce-agents) — Released Sep 2, 2026 under Apache 2.0: reference **shopping agent** and **merchant agent** built once and runnable on the Messages API, Claude Agent SDK, or Managed Agents, with four vertical examples and a Claude Code plugin to scaffold new agents. Checkout is always a hand-off to the merchant; merchant writes are staged for human approval
- [Shopify: Claude for Commerce examples](https://github.com/Shopify/claude-for-commerce-examples) — Shopify's implementation wires the shopping agent to **UCP** and **Sign in with Shop**
- [Metaverse Post](https://mpost.io/anthropic-unveils-open-source-shopping-and-merchant-agent-toolkit-with-enterprise-reference-implementations/) · [Linas Beliūnas (Substack)](https://linas.substack.com/p/claude-commerce-agents)

#### Visa, Mastercard, and Ant International Align on Know Your Agent (September 2026)

- [Business Wire: Ant International, Mastercard and Visa initiate collaboration on KYA interoperability (Sep 9, 2026)](https://www.businesswire.com/news/home/20260909003891/en/Ant-International-Mastercard-and-Visa-Initiate-Collaboration-on-Know-Your-Agent-Interoperability-to-Scale-Agentic-Commerce) — First cross-network alignment on agent identity: TAP, Verifiable Intent, and AMP to converge on common KYA principles so agents don't re-verify per network. Intent only for now — no technical spec, governance body, or timeline
- [PYMNTS](https://www.pymnts.com/cybersecurity/2026/visa-mastercard-team-with-ant-know-your-agent-framework) · [CNBC](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) · [Forkast: "Now comes the hard part"](https://forkast.news/ant-international-visa-and-mastercard-agree-on-agent-identity-standard-now-comes-the-hard-part/)

#### India: NPCI Unified Agent Protocol — Acknowledged, Not Launched, at GFF 2026 (September 2026)

- [Reuters (via Business Recorder): India preparing rollout of agentic payments on UPI (Sep 1, 2026)](https://www.brecorder.com/news/40437409/india-preparing-rollout-of-agentic-payments-on-upi-sources-say) — NPCI is preparing a **Unified Agent Protocol** that lets AI agents execute UPI payments within user-set limits **without per-transaction approval**, built on existing UPI Circle delegation and Reserve Pay rather than new rails; agents are registered, verified, and authorised as trusted parties. Media reports had anticipated an unveiling at the **Global Fintech Fest, Mumbai (Sep 8–11)** — see the correction below. First use cases: groceries and routine low-value purchases, later price-threshold ordering and investments. The first **national payment infrastructure** (rather than a company- or consortium-led standard) to open a native agentic rail — and, given UPI's scale, potentially the largest agentic payment network in the world on day one
- [Business Standard](https://www.business-standard.com/finance/news/india-may-allow-agentic-ai-led-upi-transactions-under-new-npci-protocol-126070801343_1.html) · [Inc42](https://inc42.com/buzz/npci-to-launch-agentic-payments-on-upi-report/) · [The Star (Reuters)](https://www.thestar.com.my/tech/tech-news/2026/09/01/india-preparing-rollout-of-agentic-payments-on-upi-sources-say)
- **Correction (Sep 14, 2026):** the protocol was **not** launched at GFF. NPCI chairman Ajay Kumar Choudhary said in his Sep 10 keynote that NPCI "is also examining the protocols that may be required to identify and authorise digital agents" within UPI, and set a design boundary — "AI may recommend, but authentication and final settlement must follow deterministic auditable rules." NPCI instead launched **AiNxt** (open-source agentic AI platform) and **AtOM** (signed audit-trail orchestration for UPI integration). NPCI has not published UPI technical specs publicly since 2016–17, so the first public artifact may be a member circular rather than an open spec ([MediaNama — keynote](https://www.medianama.com/2026/09/223-npci-ai-agents-upi-payments/); [MediaNama — GFF launches](https://www.medianama.com/2026/09/223-agentic-ai-products-fintechs-gff-2026/))

#### Coinbase "Agentic Finance (AiFi)" — x402 Passes 205M Transactions (August 2026)

- [Coinbase: AiFi — The Financial System for AI (Aug 27, 2026)](https://x.com/coinbase/article/2092995079640141855) — Brian Armstrong frames **Agentic Finance (AiFi)** as two tracks — agentic trading and agentic commerce — with programmable stablecoins as the native money for agents and Coinbase for Agents (MCP) as the account layer. Alongside the framing, Coinbase released updated x402 metrics: **205M cumulative agent transactions, ~$53M cumulative volume**; ~**14M transfers in the trailing 30 days** (Base 7.3M, Polygon 5.6M), with nearly all settlement in **USDC**
- [CryptoTimes](https://www.cryptotimes.io/2026/08/27/coinbase-pushes-ai-agents-into-crypto-trading-and-payments/) · [cryptonews.net (205M)](https://cryptonews.net/news/market/33360007/) · [GNCrypto (30-day breakdown)](https://www.gncrypto.news/news/coinbase-x402-14m-ai-agent-payments-usdc-base-polygon/)

#### Mastercard Start Path — Inaugural Agentic Commerce Cohort; t54 Selected (September 2026)

- [The Paypers: Mastercard Start Path adds 22 firms to agentic commerce track (Sep 2, 2026)](https://thepaypers.com/payments/news/mastercard-start-path-adds-22-firms-to-agentic-commerce-track) — First intake of the **Agentic Commerce & Services** track (created Jan 2026). Of note for this tracker: **t54** (t54 labs, x402 Foundation member; maker of **x402-secure** endpoint risk-scoring) was selected for the cohort, positioned as identity verification, risk assessment, and dispute resolution for merchants and payment networks transacting with agents. t54 also builds the **x402 facilitator on XRPL** as a Ripple partner, and that facilitator integrates Mastercard's **Verifiable Intent** — one of the first concrete bridges between the card-network trust layer (Agent Pay / AP4M / FIDO) and the stablecoin x402 rail. Other cohort members spanning the agent-payments stack: Skyfire (agent identity + payment credentials), SolvaPay, Crossmint (stablecoin wallets), Tunic Pay (agentic scam detection), PayOS, Nevermined (agent purchase settlement on existing rails), Firmly, ReFiBuy
- [The Currency Analytics: XRPL agentic transactions near 4M as t54 and Mastercard back agentic commerce (Sep 5, 2026)](https://thecurrencyanalytics.com/altcoins/xrp-ledger-ai-transactions-near-4-million-as-t54-and-mastercard-back-agentic-commerce-290849) — XRPL agentic transaction count reportedly crossed 3M on Sep 1 and neared 4M by Sep 5, driven by XRP/RLUSD-settled x402 payments via the XRPL AI Starter Kit and t54's facilitator ([CryptoBenelux](https://cryptobenelux.com/ripple-nieuws/xrp-ledger-passeert-4-miljoen-ai-betalingen-terwijl-mastercard-t54-selecteert)) · [Forkast](https://forkast.news/mastercard-start-path-launches-inaugural-agentic-commerce-cohort/) · [Yahoo Finance](https://finance.yahoo.com/technology/ai/articles/mastercard-start-path-launches-inaugural-131043302.html)

#### Amazon Bedrock AgentCore Payments Reaches GA (August 2026)

- [AWS: AgentCore payments is now generally available (Aug 18, 2026)](https://aws.amazon.com/about-aws/whats-new/2026/08/bedrock-agentcore-payments-ga/) — Moved from preview to **general availability**. GA adds **MPP protocol support** (pay any MPP-compatible service with no extra code) and the **x402 "upto" scheme** (spending ceilings instead of fixed prices), alongside Coinbase and Stripe Privy wallet integration, infrastructure-level payment limits, and end-to-end observability — the first hyperscaler to make agent payments a standard managed runtime capability
- [AWS ML Blog: GA deep dive](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale/) · [The Paypers](https://thepaypers.com/payments/news/amazon-bedrock-agentcore-payments-is-now-generally-available)

#### Rain Launches the Agentic Payments Alliance (August 2026)

- [Rain: Agentic Payments Alliance launch (Aug 18, 2026)](https://www.prnewswire.com/news-releases/rain-launches-the-agentic-payments-alliance-to-guide-the-future-of-agent-driven-commerce-302853532.html) — 26 founding members including **Visa, Mastercard, Circle, Fiserv, Fireblocks, Shift4, Solana, Uniswap Labs, Chainalysis, and Remitly**, developing shared standards for agent identity, authorization, fraud, and programmable payments — the first governance coalition spanning both card networks and crypto-native infrastructure. Only 7 members overlap with the x402 Foundation, underscoring how fragmented standards governance remains ([HaiPay analysis](https://www.haipay.net/news/agentic-payments-alliance-x402-membership-overlap))
- [PYMNTS](https://www.pymnts.com/news/artificial-intelligence/2026/visa-and-mastercard-join-rains-agentic-commerce-coalition/) · [Electronic Payments International](https://www.electronicpaymentsinternational.com/news/rain-forms-agentic-payments-alliance-with-visa-mastercard-and-other-players/)

#### Stripe Agrees to Acquire OpenRouter (August 2026)

- [Stripe: agreement to acquire OpenRouter (Aug 16, 2026)](https://stripe.com/newsroom/news/stripe-agrees-to-acquire-openrouter) — Stripe's largest known acquisition (**$7B+** per Bloomberg), bringing in the gateway that routes traffic across 400+ models from 80+ providers. Extends Stripe's agentic stack beyond money movement into the **model-consumption/token-metering layer** — one commercial stack for metering AI usage, selecting inference providers, and monetizing agent-facing services
- [TechCrunch](https://techcrunch.com/2026/08/16/stripe-will-reportedly-acquire-ai-gateway-startup-openrouter-for-7b/) · [The New Stack](https://thenewstack.io/stripe-acquires-openrouter-tokens/)

#### Cloudflare Agents Week — Programmable Agent Wallets + WebMCP (August 2026)

- [Cloudflare: programmable wallets for AI agents](https://blog.cloudflare.com/wallets/) — Developers provision **stablecoin-backed wallets to accounts and virtual wallets to individual agents**, with spending allowances, transaction limits, and merchant restrictions; pairs x402-compatible machine payments with delegated identity so merchants can distinguish authorized agents from unidentified automation
- [Cloudflare: WebMCP developer preview](https://blog.cloudflare.com/webmcp/) — Site operators expose structured browser-agent actions (search, cart, authenticated workflows) without building a separate API — complements Chrome's WebMCP origin trial
- Also shipped: [Agent Readiness + Answer Engine Optimization tooling](https://blog.cloudflare.com/aeo/) (measure whether agents can discover/interpret a site and how often assistants recommend it), [WriteGuard private beta](https://blog.cloudflare.com/mcp-portal-writeguard-private-beta/) (least-privilege authorization for MCP write operations), and the [Agent Access Model](https://blog.cloudflare.com/the-agent-access-model/) (task-scoped delegated authority)

#### Mastercard Proto Sandbox Goes Live in the UK (August 2026)

- [Finextra: Mastercard picks UK for agentic AI sandbox](https://www.finextra.com/newsarticle/48097/mastercard-picks-uk-as-test-environment-for-agentic-ai-sandbox) — **Proto**, Mastercard's agentic commerce sandbox, goes live in the UK in August (announced Jul 16) so retailers and financial institutions can test agent discoverability, trusted payment flows, and dispute handling at scale before launch; includes three new enterprise agents (shopping, onboarding, disputes)
- [Payment Expert](https://paymentexpert.com/2026/07/16/mastercard-ai-sandbox-uk-payments/) · [Mastercard Newsroom](https://www.mastercard.com/news/europe/en-uk/perspectives/en-gb/helping-the-uk-get-ai-ready/)

#### An Accountability Layer Emerges — LCP and A-Comm Evidence Protocol (June–July 2026)

- [AAA and Integra Ledger launch the Legal Context Protocol (Jun 24, 2026)](https://www.adr.org/press-releases/aaa-and-industry-leaders-launch-legal-protocol-for-agentic-commerce/) — Verifiable legal terms, consent, and dispute-resolution procedure attached to agent transactions; founding contributors include Google, IBM, Circle, and Wayfair ([Law.com](https://www.law.com/legaltechnews/2026/06/24/aaa-and-integra-ledger-announce-legal-protocol-for-ai-agent-transactions-/))
- [A-Comm opens public comment on its Evidence Protocol (Jul 13, 2026)](https://www.prnewswire.com/news-releases/a-comm-technologies-inc-opens-public-comment-on-evidence-standard-for-agentic-commerce-302829047.html) — Tamper-evident evidence chain for AI-initiated consumer transactions; **comment window closes Aug 14, 2026** ([Digital Transactions](https://www.digitaltransactions.net/a-comms-agentic-prep-and-other-digital-transactions-news-briefs-from-7-20-26/))
- Read alongside [RAILS (arXiv, Jun 7, 2026)](https://arxiv.org/abs/2606.08790). Three unconnected efforts — an arbitration body, a payments startup, and an academic paper — arriving at the same conclusion within six weeks is the signal: the 2026 protocol race optimized settlement and left post-transaction accountability unspecified

#### x402 Foundation Operational Launch — 40 Members (July 2026)

- [Linux Foundation: operational launch of the x402 Foundation](https://www.linuxfoundation.org/press/linux-foundation-announces-operational-launch-of-x402-foundation-to-standardize-internet-native-payments-for-ai-agents-and-applications) — Announced Jul 14; Coinbase's contribution of the protocol **completed**; 40 members seated (17 premier, incl. Stripe, Visa, Mastercard, Google, AWS, Amex, Circle, Cloudflare, Fiserv, Ripple, Shopify, Solana Foundation, Stellar)
- [PRNewswire](https://www.prnewswire.com/news-releases/linux-foundation-announces-operational-launch-of-x402-foundation-to-standardize-internet-native-payments-for-ai-agents-and-applications-302824778.html) · [PYMNTS](https://www.pymnts.com/news/2026/40-finance-and-tech-giants-unite-to-standardize-agentic-payments/) · [cfotech](https://cfotech.news/story/linux-foundation-launches-x402-foundation-with-40-members)

#### Visa — Live Agentic Commerce in Europe (July 2026)

- [Visa: Banks across Europe reach the next phase of agentic commerce](https://www.visa.co.uk/about-visa/newsroom/press-releases.3457328.html) — First *live* agentic transactions with 30+ European issuers at real merchants (lastminute.com, Frasers, Cleverbridge, BrickDepot), via Visa Intelligent Commerce + Payment Passkeys; announced at Visa Payments Forum, Paris (Jul 2)
- [Payment Expert](https://paymentexpert.com/2026/07/02/visa-agentic-payments-merchants-eu/) · [Worldline/ING/Visa live transaction](https://www.globenewswire.com/news-release/2026/07/02/3321259/0/en/WORLDLINE-Worldline-ING-and-Visa-complete-a-live-agentic-payment-transaction-in-Europe-Press-release.html)

#### Nuvei Agentic — Merchant-Led Strategy + First In-Agent Visa Payment (July 2026)

- [Nuvei: first-party in-agent payment with Visa; merchant-led agentic strategy](https://www.nuvei.com/posts/nuvei-completes-first-party-in-agent-payment-with-visa-unveils-merchant-led-agentic-payments-strategy) — Protocol Compatibility Layer (integrate once; accept ACP/AP2/MCP) + Know Your Agent registry; first-party in-agent payment on live Visa rails (Arvato Systems, Kings and Priests); GA targeted H2 2026 (Jul 2)
- [The Paypers](https://thepaypers.com/payments/news/nuvei-completes-its-first-in-agent-payment-on-visa-rails) · [PR Newswire](https://www.prnewswire.com/news-releases/nuvei-completes-first-party-in-agent-payment-with-visa-unveils-merchant-led-agentic-payments-strategy-302816873.html)

#### Square — In-Agent Ordering via ChatGPT App + Claude Plugin (July 2026)

- [Square: ChatGPT and Claude integrations for sellers](https://squareup.com/us/en/press/claude-chatgpt-integrations) — From Jul 1, Square Food & Beverage sellers with an active Square Online Ordering profile are **auto-enrolled** so shoppers can browse menus and order directly inside ChatGPT and Claude; orders route through Square's "Order by Cash App" rails with **no marketplace commission** (vs. 15–30% for delivery apps) — only standard processing. Square positions itself as the low-fee payment + fulfillment layer under multiple assistants rather than building its own ([VentureBeat](https://venturebeat.com/technology/restaurants-can-now-accept-orders-placed-directly-from-chatgpt-and-claude-thanks-to-squares-new-low-fee-no-setup-integration), [Cryptobriefing](https://cryptobriefing.com/square-chatgpt-claude-restaurant-orders/))

#### Cloudflare Monetization Gateway (July 2026)

- [Cloudflare: Announcing the Monetization Gateway](https://blog.cloudflare.com/monetization-gateway/) — Sell-side x402 product to charge for web pages, datasets, APIs, and MCP tools with stablecoin settlement at the edge; waitlist opened Jul 1
- [InfoQ: Cloudflare and AWS embed x402 at the edge](https://www.infoq.com/news/2026/07/cloudflare-aws-x402-micropayment/) · [crypto.news](https://crypto.news/cloudflare-opens-waitlist-for-x402-stablecoin-monetization-gateway/)

#### Open USD (OUSD) Stablecoin Consortium (June 2026)

- [Fortune: Stripe, Visa and 140+ businesses to launch Open USD](https://fortune.com/2026/06/30/stripe-visa-stablecoin-rival-ousd-tether-circle/) — Shared-governance USD stablecoin backed by 140+ firms (Stripe, Visa, Mastercard, Coinbase, BlackRock, BNY, Google, Shopify, Fireblocks, Aave, Solana); fee-free mint/redeem, member-shared reserve income; live on Solana, Stellar, Base, Polygon later in 2026
- [CoinDesk](https://www.coindesk.com/business/2026/06/30/circle-slides-8-as-stripe-coinbase-and-blackrock-back-rival-stablecoin-network) · [Forrester](https://www.forrester.com/blogs/stripes-new-stablecoin-bet-open-usd/)

#### Mastercard Agent Pay for Machines (AP4M) (June 2026)

- [Mastercard: Agent Pay for Machines launch](https://www.mastercard.com/us/en/news-and-trends/press/2026/june/mastercard-launches-agent-pay-for-machines.html) — Network for high-frequency, low-value machine-to-machine payments; on-chain agent credentials (Polygon/Solana/Base), Verifiable Intent, fiat or stablecoin settlement, 30+ partners
- [Fortune](https://fortune.com/2026/06/10/mastercard-ai-payments-protocol-launch-agentic-finance/) · [CoinDesk](https://www.coindesk.com/business/2026/06/10/mastercard-prepares-for-a-future-where-ai-agents-make-payments-with-latest-introduction)

#### Coinbase for Agents (June 2026)

- [Coinbase: Coinbase for Agents](https://www.coinbase.com/blog/coinbase-for-agents) — MCP server letting ChatGPT/Claude agents transact via a Coinbase account, paying for premium research/compute over x402
- [TechCrunch](https://techcrunch.com/2026/06/11/coinbase-debuts-mcp-for-agent-trading/)

#### Ripple XRPL AI Starter Kit (June 2026)

- [Ripple: XRPL AI Starter Kit](https://ripple.com/insights/xrpl-ai-starter-kit/) — Agentic payments on XRPL via x402 with XRP/RLUSD settlement; XRPL Docs MCP server + Claude skills
- [PYMNTS](https://www.pymnts.com/blockchain/2026/ripple-targets-agentic-payments-market-with-xrpl-starter-kit/)

#### Adyen Agentic (June 2026)

- [Adyen: Adyen Agentic](https://www.adyen.com/press-and-media/adyen-agentic) — Three-layer, protocol-agnostic suite (Agentic Feed/Cart/Payments) for selling through AI agents
- [PYMNTS](https://www.pymnts.com/news/b2b-payments/2026/adyen-debuts-agentic-solutions-for-enterprise-merchants/)

#### Visa × OpenAI: Agent Payments in ChatGPT (June 2026)

- [Axios: Visa, OpenAI bring agentic commerce to ChatGPT](https://www.axios.com/2026/06/10/visa-chatgpt-agents-commerce) — Visa payment tools integrated into OpenAI's agent system for tokenized agent checkout

#### AP2 Donated to FIDO Alliance + v0.2 (April–May 2026)

- [Google: Donating AP2 to the FIDO Alliance](https://blog.google/products-and-platforms/platforms/google-pay/agent-payments-protocol-fido-alliance/) — Community governance; v0.2 adds "Human Not Present" payments and Verifiable Intent
- [FIDO Alliance](https://fidoalliance.org/google-donates-agent-payments-protocol-to-fido-alliance/) · [PaymentsJournal](https://www.paymentsjournal.com/google-donates-its-agentic-payments-protocol-to-the-fido-alliance/)

#### x402 Foundation Joins the Linux Foundation (April 2026)

- [Linux Foundation: launching the x402 Foundation](https://www.linuxfoundation.org/press/linux-foundation-is-launching-the-x402-foundation-and-welcoming-the-contribution-of-the-x402-protocol) — Coinbase contributes x402 for neutral governance; founding contributors Coinbase, Cloudflare, Stripe
- [Decrypt](https://decrypt.co/363173/coinbase-linux-foundation-launch-x402-foundation) · [The Block](https://www.theblock.co/post/396155/tech-crypto-giants-to-help-steward-coinbases-neutral-x402-payments-protocol-under-linux-foundation)
- *Superseded by the July 2026 operational launch — see above*

#### Alipay Agentic Commerce Trust Protocol + AI Pay at Scale (Jan–Feb 2026)

- [The Paypers: Alipay rolls out the Agentic Commerce Trust Protocol](https://thepaypers.com/payments/news/alipay-rolls-out-the-agentic-commerce-trust-protocol-in-china) — Launched with Qwen App and Taobao Instant Commerce
- [Business Wire: Alipay AI Pay exceeds 120M transactions in one week](https://www.businesswire.com/news/home/20260213770962/en/Alipay-AI-Payment-Exceeds-120-Million-Transactions-in-One-Week-as-Agentic-Commerce-Accelerates-in-China) · [FinTech Magazine](https://fintechmagazine.com/news/alipay-hits-120m-weekly-ai-agent-transactions) · [Retail Technology Innovation Hub](https://retailtechinnovationhub.com/home/2026/2/12/alipay-ai-pay-solution-exceeds-120m-transactions-as-agentic-commerce-accelerates-in-china)

#### Amazon Bedrock AgentCore Payments (Preview, May 2026)

- [AWS What's New: AgentCore Payments (preview)](https://aws.amazon.com/about-aws/whats-new/2026/04/amazon-bedrock-agentcore-payments-preview/)
- [AWS ML Blog: Agents that transact, built with Coinbase and Stripe](https://aws.amazon.com/blogs/machine-learning/agents-that-transact-introducing-amazon-bedrock-agentcore-payments-built-with-coinbase-and-stripe/)
- [Coinbase Blog: AgentCore Payments powered by x402](https://www.coinbase.com/blog/introducing-amazon-bedrock-agentcore-payments-powered-by-x402-and-coinbase)
- *Superseded by the August 2026 GA — see above*

#### Google Gemini Spark (Google I/O, May 2026)

- [Gemini Spark announced (Yahoo Tech)](https://tech.yahoo.com/ai/gemini/articles/googles-gemini-spark-announced-meet-174500393.html) — Consumer AP2 agent surface with autonomous, guardrailed purchasing
- [Google I/O 2026 recap (TheTechHacker)](https://thetechhacker.com/2026/05/20/google-io-2026-recap-gemini-flash-autonomous-agent/)

#### Ant International Launches AMP (April 2026)

- [Business Wire: Ant International launches open-sourced Agentic Mobile Protocol](https://www.businesswire.com/news/home/20260427209524/en/Ant-International-Launches-Open-Sourced-Agentic-Mobile-Protocol-to-Drive-AI-Commerce) — Mobile-native agentic payments via Alipay+

#### OpenAI Discontinues Instant Checkout, Pivots ACP to Discovery (Q1 2026)

- [OpenAI: Powering Product Discovery in ChatGPT (Mar 24, 2026)](https://openai.com/index/powering-product-discovery-in-chatgpt/) — The pivot in OpenAI's own words: ACP extended to discovery; Target, Sephora, Nordstrom, Lowe's, Best Buy, The Home Depot, and Wayfair integrated; all Shopify merchants included via Shopify Catalog; Walmart in-ChatGPT app with account linking, loyalty, and Walmart payments
- [TechCrunch: OpenAI's plans to make ChatGPT more like Amazon aren't going so well](https://techcrunch.com/2026/03/24/openais-plans-to-make-chatgpt-more-like-amazon-arent-going-so-well/)
- [CNBC: OpenAI's first crack at online shopping stumbled — preparing for the next wave](https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html)
- [Grocery Dive: Walmart brings Sparky to ChatGPT](https://www.grocerydive.com/news/walmart-sparky-chatgpt-instant-checkout/815961/)

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
- [Inside x402: agentic payments on Base (Chainalysis)](https://www.chainalysis.com/blog/x402-agentic-payments-adoption/) — 100M milestone in Q1 2026, climbing to **~169M cumulative** by July 2026 · [Base adds 20M transfers in 90 days; 169M total (Cryptobriefing)](https://cryptobriefing.com/base-agentic-payments-20-million-transfers/)

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
- [CoinDesk: Meta's Chief Data Officer says agentic commerce is the "next tier of business" (Jul 10, 2026)](https://www.coindesk.com/coindesk-news/2026/07/10/meta-s-chief-data-officer-says-agentic-commerce-is-the-next-tier-of-business) — Meta CDO Alex Schultz frames agentic commerce as a company-level priority, positions **stablecoins** as the payments layer (1M+ weekly-active businesses already using Meta agents), and names **agent identity/verification** as the core unsolved problem for an agent-to-agent economy
- [PYMNTS: Agentic payments give CFOs usage pricing with subscription discipline (Jul 8, 2026)](https://www.pymnts.com/news/artificial-intelligence/2026/agentic-payments-give-cfos-usage-pricing-with-subscription-discipline/) — The **"agentic administration"** thesis: the first serious enterprise use of agent payments is wholesale/back-office (API calls, software usage, data checks) rather than consumer retail; enterprises need batch settlement, spend limits, and auditable reconciliation — echoing Cloudflare's Monetization Gateway positioning

### Security & Standards

- [Cloud Security Alliance: Secure Use of AP2](https://cloudsecurityalliance.org/blog/2025/10/06/secure-use-of-the-agent-payments-protocol-ap2-a-framework-for-trustworthy-ai-driven-transactions)
- [PayPal Dev Blog: AP2 mandates as W3C VCs](https://developer.paypal.com/community/blog/PayPal-Agent-Payments-Protocol/)
- [IETF charters the Web Bot Auth working group (`webbotauth`)](https://datatracker.ietf.org/wg/webbotauth/about/) — Agent identity via HTTP Message Signatures graduates from individual drafts to a chartered WG under the Web and Internet Transport area, with standards-track and BCP deliverables due to the IESG in 2026. The charter's explicit exclusion of agent-to-agent interfaces and end-user authentication marks the seam between Web Bot Auth and the payment-mandate protocols

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

**UCP (Universal Commerce Protocol)** is an open standard co-developed by Google and Shopify for agentic commerce across the full shopping journey — discovery, checkout, identity linking, and order management. UCP is transport-agnostic (REST, MCP, A2A) and compatible with AP2 for secure payment mandates. Launched January 2026 at NRF; Universal Cart — a cross-merchant cart spanning Search, Gemini, YouTube, and Gmail with UCP-powered Google Pay checkout — added May 2026, rolling out in the U.S. over summer 2026 with Canada, Australia, and the U.K. to follow.

**AP2 (Agent Payments Protocol)** is an open protocol for agent-driven payments with verifiable authorization (mandates) and accountability, created by Google and **donated to the FIDO Alliance for community governance in 2026**. Its current core focus is card-based payments with mandate-driven authorization; the v0.2 release added "Human Not Present" payments and Verifiable Intent (co-developed with Mastercard). AP2 serves as the payment layer within UCP.

**A2A (Agent-to-Agent Protocol)** is an open standard under the Linux Foundation for agent interoperability — discovery, communication, and task delegation across agent frameworks and vendors. The v1.0 release (2026) added enterprise features including signed agent cards, multi-tenancy, and version negotiation. The TSC includes AWS, Cisco, Google, IBM Research, Microsoft, Salesforce, SAP, and ServiceNow.

**x402** is an open payment standard built on HTTP 402 for machine-native, internet-native payments. Created by Coinbase and governed by the x402 Foundation under the **Linux Foundation** — announced April 2026 (founding contributors Coinbase, Cloudflare, and Stripe) and operationally launched **July 14, 2026** with 40 members, including Stripe, Visa, Mastercard, Google, AWS, and American Express among 17 premier members. Supports stablecoins on EVM and Solana networks. The v2 release (late 2025) introduced CAIP-based identifiers, a modular SDK architecture, and standards-compliant payment headers. By mid-2026 it is wrapped by managed surfaces such as AWS Bedrock AgentCore; per Coinbase (Aug 2026) it has surpassed 205M cumulative agentic transactions (~$53M volume), settled almost entirely in USDC on Base and Polygon.

**ACP (Agentic Commerce Protocol)** is an open standard co-developed by OpenAI and Stripe for connecting buyers, AI agents, and businesses. It originally powered Instant Checkout in ChatGPT; after that consumer experience was discontinued in early 2026, OpenAI repositioned ACP as a **discovery-and-handoff layer** — merchants supply product feeds and promotions into ChatGPT, and shoppers complete purchases on the merchant's own site. Target, Sephora, Nordstrom, Lowe's, Best Buy, The Home Depot, and Wayfair are integrated for discovery, with all Shopify merchants included automatically via Shopify Catalog. Deeper integrations are built as ChatGPT apps (e.g. Walmart). Currently in beta with date-based version snapshots. Designed to work with any PSP — Stripe provides the first implementation via Shared Payment Token.

**MPP (Machine Payments Protocol)** is an open standard co-authored by Tempo Labs and Stripe for machine-to-machine payments over HTTP 402. Supports stablecoins, cards, and bank transfers. Offers `charge` (one-off) and `session` (streaming micropayment) intents. Backwards-compatible with x402. Based on an IETF-proposed Payment HTTP Authentication Scheme. Launched March 2026.

**AMP (Agentic Mobile Protocol)** is an open-sourced framework from Ant International for agentic payments on mobile surfaces — digital wallets, super apps, banking apps, and wearables. Implemented via Alipay+, it emphasizes fast agent-to-wallet linking (~50% fewer steps than card binding) and account-takeover protection with a per-transaction money-back guarantee. Launched April 2026.

**Agentic Commerce Trust Protocol (Alipay)** is Alipay's domestic-China integration layer between AI-native applications and merchant/service platforms, launched January 2026 with Alibaba's Qwen App as first adopter alongside Taobao Instant Commerce. One merchant integration reaches multiple AI agents without per-agent API work. Settlement runs through **Alipay AI Pay**, which passed **120M transactions in a single week** in February 2026 — the largest agentic payment deployment in production, and a reminder that the highest-volume agentic commerce today is happening outside the US/EU protocol race.

**Trusted Agent Protocol (Visa) / Agent Pay (Mastercard)** help merchants and networks recognize cryptographically verified AI agents during browse and pay flows, built on **Web Bot Auth**, which became a chartered IETF working group (`webbotauth`) in 2026. Both expanded internationally in 2026, and in July 2026 Visa executed the first live agentic-commerce transactions in Europe (30+ issuers, via Visa Intelligent Commerce and Payment Passkeys). In 2026 Visa also released an open, processor-agnostic card specification and SDK extending MPP to card payments. In June 2026 Mastercard launched **Agent Pay for Machines (AP4M)**, a dedicated network for high-frequency machine-to-machine payments using on-chain agent credentials and Verifiable Intent, settling in fiat or stablecoin.

**The accountability layer (AEP / LCP / RAILS)** is the newest and least consolidated part of the stack. Where the protocols above answer *how does an agent pay*, these answer *what happens when the transaction is contested* — a question the settlement standards leave open by design. The **A-Comm Evidence Protocol** produces a tamper-evident record of what an agent did at each step; the **Legal Context Protocol**, stewarded by the American Arbitration Association and Integra Ledger, attaches the governing legal terms and dispute procedure to the transaction itself; and **RAILS** supplies the academic framing, arguing that clearing — a neutral determination of whether a delegated obligation was met — is the primitive the whole stack is missing. None of the three competes with x402, ACP, UCP, AP2 or the card-network rails; all three assume those rails and sit downstream of them. Whether they converge, get absorbed by the card networks' dispute machinery, or remain parallel experiments is the open question going into late 2026.

---

## 📄 License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under [CC0 1.0](LICENSE) (Public Domain). No rights reserved.

---

**Keywords:** `ucp` `ap2` `agent-payments` `agentic-commerce` `a2a` `x402` `acp` `mpp` `machine-payments-protocol` `amp` `agentic-mobile-protocol` `trusted-agent-protocol` `agent-pay` `ap4m` `agent-pay-for-machines` `verifiable-intent` `fido-alliance` `linux-foundation` `adyen-agentic` `open-usd` `ousd` `sekau` `visa-payment-passkeys` `monetization-gateway` `pay-per-crawl` `gemini-spark` `web-bot-auth` `mcp` `stablecoins` `verifiable-credentials` `agentcore` `erc-8183` `erc-8004` `google-cloud` `coinbase` `stripe` `openai` `aws` `tempo` `ripple` `xrpl` `rlusd` `nuvei-agentic` `know-your-agent` `webmcp` `circle-arc` `agent-stack` `agentic-administration` `x402-foundation` `universal-cart` `alipay-ai-pay` `agentic-commerce-trust-protocol` `qwen-app` `shopify-catalog` `webbotauth` `ietf` `http-message-signatures` `aep` `a-comm` `evidence-protocol` `legal-context-protocol` `lcp` `integra-ledger` `aaa-arbitration` `rails` `agentic-clearing` `accountability-layer` `ucp-tech-council` `visa-agent-directory` `square-ordering` `order-by-cash-app` `acp-2026-04-17` `agentic-payments-alliance` `rain` `openrouter` `proto-sandbox` `agentcore-ga` `mppx` `cloudflare-agent-wallets` `binance-agent-os` `glassnode` `upto-scheme` `permit2` `trust-before-spend` `t54-x402-secure` `t54` `unified-agent-protocol` `npci` `upi-circle` `aifi` `agentic-finance` `start-path` `xrpl-facilitator`
