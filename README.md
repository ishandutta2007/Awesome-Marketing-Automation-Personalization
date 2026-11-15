# Awesome-Marketing-Automation-Personalization

# Awesome Marketing Automation & Personalization

> A curated list of top Marketing Automation and Personalization platforms — both SaaS/Hosted commercial solutions and open-source alternatives for automating campaigns, segmenting audiences, and delivering personalized experiences.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [HubSpot Marketing Hub](#hubspot-marketing-hub)
  - [ActiveCampaign](#activecampaign)
  - [Marketo Engage](#marketo-engage)
  - [Klaviyo](#klaviyo)
  - [Braze](#braze)
  - [CleverTap](#clevertap)
- [Open-Source Software](#-open-source-software)
  - [Mautic](#mautic)
  - [Dittofeed](#dittofeed)
  - [Helio](#helio)
  - [Tracardi](#tracardi)
  - [LEO CDP](#leo-cdp)
  - [Apache Unomi](#apache-unomi)
  - [Listmonk](#listmonk)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Marketing Automation and Personalization platforms. These are not open-source but are included as reference points for feature comparison.

### HubSpot Marketing Hub
**Type:** All-in-one marketing platform with CRM integration
HubSpot Marketing Hub provides email marketing, social media, landing pages, forms, automation workflows, and analytics, tightly integrated with HubSpot CRM. It is the natural choice for organizations already using HubSpot, with a free tier for basic email marketing and paid tiers scaling by contacts and features.

### ActiveCampaign
**Type:** Marketing automation with integrated CRM
ActiveCampaign combines email marketing, marketing automation, and a lightweight CRM, known for automation depth relative to price. It supports email, SMS, and site messaging, with pricing starting at $15/month for the Starter plan and scaling by contacts.

### Marketo Engage
**Type:** Enterprise marketing automation within Adobe
Marketo Engage (Adobe) provides sophisticated B2B marketing automation with lead scoring, multi-touch attribution, account-based marketing, and complex campaign orchestration. It is positioned for large enterprises with complex B2B sales cycles, with pricing that targets enterprise budgets.

### Klaviyo
**Type:** E-commerce marketing automation
Klaviyo specializes in email and SMS marketing for e-commerce, with deep integrations into Shopify, WooCommerce, and BigCommerce for behavioral triggers and segmentation. It is positioned for DTC brands wanting revenue-attributed campaigns, with pricing scaling by contacts.

### Braze
**Type:** Enterprise cross-channel customer engagement platform
Braze is consistently positioned as a Leader in Gartner's Magic Quadrant for Multichannel Marketing Hubs, alongside Adobe, Salesforce, and SAP. It provides journey orchestration, cross-channel messaging (email, push, SMS, in-app, webhooks), and real-time segmentation, with a strong focus on mobile-first engagement. Pricing is enterprise-quoted and scales with monthly active users.

### CleverTap
**Type:** Mobile-first engagement and retention platform
CleverTap is included in Gartner's Magic Quadrant and the QKS SPARK Matrix for Multichannel Marketing Hubs. It focuses on mobile app engagement, with push notifications, in-app messages, and retention analytics. Positioned for consumer apps with large mobile user bases.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Marketing Automation and Personalization tools. The open-source ecosystem spans **mature marketing automation platforms**, **modern developer-friendly engagement suites**, **AI-native growth platforms**, **composable CDP engines**, and **real-time personalization infrastructure**.

### Mautic
**Stack:** PHP / MySQL | **License:** GPL-3.0
Mautic is the world's largest open-source marketing automation project, explicitly positioned for data sovereignty and privacy . Key capabilities include:
- **Multi-channel marketing**: email, SMS, app or browser notifications out of the box, with more channels via plugins
- **Visual campaign builder**: drag-and-drop journey orchestration with conditional logic
- **Lead management**: scoring, stages, and behavioral tracking
- **GDPR compliance**: consent management, data erasure, and audit logs
- **Unlimited users**: no per-seat pricing
- **REST API** for CRM integration
- **Self-hosted** with full data control

**Critical deployment detail:** A dedicated cron worker is required for campaigns and scheduled emails to actually fire—the most common failure in self-hosted Mautic deployments. Mautic is a direct alternative to HubSpot, ActiveCampaign, and Mailchimp, with no per-contact pricing [citation:2][citation:10].
**Best for:** Organizations wanting a proven, privacy-focused marketing automation platform with full data ownership and no per-user fees, accepting the PHP/MySQL deployment and cron configuration.

### Dittofeed
**Stack:** TypeScript / Node.js | **License:** Open Source (core)
Dittofeed is an open-source customer engagement platform offering low-code tools for message automation across multiple channels, including powerful segmentation and personalization features [citation:2][citation:10]. It is positioned as a modern, developer-friendly alternative to commercial engagement platforms, with a focus on event-triggered journeys and user segmentation.
**Best for:** Developer teams wanting a modern, TypeScript-based engagement platform with git workflows and CI testing, accepting the self-hosted deployment.

### Helio
**Stack:** TypeScript / Temporal / PostgreSQL / ClickHouse | **License:** AGPL-3.0
Helio is an open-source, AI-native growth platform combining a CDP, visual journey orchestration, and multi-channel delivery [citation:9]. Key capabilities include:
- **Multi-channel**: email, SMS (Twilio), WhatsApp (Cloud API), web push, and in-app messages
- **Visual journey builder**: React Flow canvas compiled to a validated DAG, with durable execution via Temporal
- **AI copilot**: describe a segment, journey, or email in a sentence and get a working draft
- **Bring your own AI**: OpenAI, Anthropic, Groq, NVIDIA NIM, or local Ollama
- **MCP server**: exposes capabilities as tools for external AI agents
- **Predictive lead scoring & churn**: with per-workspace conversion events
- **Free forever**: no plans, no contact caps, no metering

It is explicitly positioned as a Mautic alternative with AI-native capabilities [citation:9].
**Best for:** Teams wanting a genuinely free, AI-native marketing automation platform with durable execution and multi-channel delivery, accepting a newer project than Mautic.

### Tracardi
**Stack:** Python / Docker | **License:** MIT with Common Clause
Tracardi is an API-first, composable open-source **Customer Data Platform (CDP) engine** positioned as an alternative to Segment and RudderStack [citation:4]. Key capabilities include:
- **Collect customer data** from multiple sources in real time
- **Model customer data** with rules that copy data into user profiles
- **Personalize user experience** with real-time frontend apps, customized messages, and marketing segmentation
- **Unify profiles** by merging customer data from various sources
- **Integrate internal systems** as a centralized communication and orchestration hub
- **Social engagement** via bridges to e-commerce platforms

**Important licensing note:** MIT with Common Clause, which restricts certain commercial uses [citation:4].
**Best for:** Teams wanting to build a custom CDP foundation with full control over customer data collection, unification, and activation.

### LEO CDP
**Stack:** Python / Big Data / ML | **License:** Open Source
LEO CDP is an open-source, AI-first Customer Data Platform framework for building customizable, self-hosted, privacy-friendly CDP infrastructure [citation:15]. Key capabilities include:
- **Omnichannel data collection**: websites, mobile apps, CRM, POS, e-commerce, social media, APIs
- **Real-time Customer 360**: behavioral, transactional, demographic, and engagement data
- **AI-based segmentation**: RFM analysis, CLV, churn prediction, purchase propensity, lead scoring
- **Behavioral tracking and journey mapping**
- **Real-time audience activation** across marketing, sales, and advertising platforms
- **Omnichannel personalization with Agentic AI & LLMs**: AI-generated content, next-best-action, dynamic journey orchestration
- **Enterprise security**: consent management, RBAC, audit logs, multi-tenant, Docker/Kubernetes support

**Best for:** Organizations wanting an AI-native CDP with predictive analytics and LLM-powered personalization, accepting a comprehensive Python/big-data stack.

### Apache Unomi
**Stack:** Java / Apache Karaf | **License:** Apache-2.0
Apache Unomi is an open-source **customer data platform** for managing customer, lead, and visitor data [citation:12]. The City of Munich uses Unomi to personalize web content in Magnolia—for example, on stadt.muenchen.de—for specific user groups and to offer them personalized content tailored to their needs [citation:12]. It provides a REST API for managing profiles, segments, and events, with built-in privacy and consent management.
**Best for:** Organizations wanting a proven, Apache-governed CDP for web personalization and segmentation, accepting a Java-based deployment.

### Listmonk
**Stack:** Go / PostgreSQL | **License:** AGPL-3.0
Listmonk is a standalone, self-hosted **newsletter and mailing list manager** with a fast, clean interface. It supports multi-list management, custom subscriber attributes, segmentation, templates (HTML or Markdown), analytics, and transactional messaging via a REST API. It is designed for high-volume sending (millions of subscribers) with a single binary deployment and no external dependencies beyond PostgreSQL [citation:3]. It is explicitly **email-only**—no SMS, push, or journey builder.
**Best for:** Organizations wanting a lightweight, high-performance newsletter platform with segmentation and templates, accepting that it is email-only.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Multi-Channel | Visual Journey Builder | Self-Hosted | Best For |
|----------|---------|-------|---------------|------------------------|-------------|----------|
| **HubSpot** | Proprietary | Cloud | ✅ | ✅ | ❌ | HubSpot CRM integration |
| **ActiveCampaign** | Proprietary | Cloud | ✅ | ✅ | ❌ | Automation depth |
| **Braze** | Proprietary | Cloud | ✅ | ✅ | ❌ | Enterprise cross-channel |
| **Mautic** | GPL-3.0 | PHP/MySQL | ✅ Email/SMS/Notifications | ✅ Drag-and-drop | ✅ | Proven OSS + data sovereignty |
| **Dittofeed** | Open Source | TypeScript | ✅ Low-code automation | ✅ Segmentation | ✅ | Developer-friendly engagement |
| **Helio** | AGPL-3.0 | TypeScript/Temporal | ✅ Email/SMS/WhatsApp/Push | ✅ React Flow | ✅ | AI-native + free forever |
| **Tracardi** | MIT + Clause | Python/Docker | (CDP engine) | (Via rules) | ✅ | Composable CDP foundation |
| **LEO CDP** | Open Source | Python/Big Data | ✅ Omnichannel | ✅ Journey mapping | ✅ | AI-native CDP + LLM personalization |
| **Apache Unomi** | Apache-2.0 | Java | (CDP) | (Segments) | ✅ | Web personalization + segmentation |
| **Listmonk** | AGPL-3.0 | Go/Postgres | ❌ (Email only) | ❌ | ✅ | High-volume newsletters |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Marketing Automation or Personalization tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with Tracardi's Common Clause).

**Note on the open-source ecosystem:** The marketing automation and personalization space is **led by Mautic** for maturity and adoption (10k+ stars, active weekly development, proven as a HubSpot alternative for early-stage founders [citation:3]). A newer generation of modern, developer-friendly platforms has emerged: **Dittofeed** offers low-code multi-channel automation with segmentation [citation:2], **Helio** provides an AI-native growth platform with durable execution and a free-forever model [citation:9], and **Tracardi** delivers a composable CDP foundation under an open architecture [citation:4]. For **personalization specifically**, **Apache Unomi** is a proven CDP used by the City of Munich for web content personalization [citation:12], while **LEO CDP** offers an AI-first CDP with predictive analytics and LLM-powered personalization [citation:15]. No single open-source project fully replicates Braze's enterprise-scale cross-channel orchestration, but these tools cover the core automation and personalization workflows for self-hosted deployments.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
