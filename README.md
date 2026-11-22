# 👋 nordic

I build web applications, APIs, and databases. My work spans the interface people use, the services behind it, and the infrastructure that keeps it running.

## 🧾 Products and the problems they solve

| Project | What someone uses it for | Engineering concern |
| --- | --- | --- |
| Trokano | Buy or sell a digital item with payment held until delivery | Keeping inventory, order status, and the seller’s balance consistent |
| Trustly MM | Coordinate an escrow trade without leaving the Discord conversation | Sharing deal state between the bot, the API, and the dashboard |
| FlarkFPS | Review Windows performance settings and manage a desktop license | Preserving the original system settings and validating activation on the server |
| Flark Group | Explore the bilingual product catalog | Publishing the same catalog in Portuguese and English |

## 🛍️ What a marketplace order involves

Trokano connects three perspectives on one purchase. A buyer sees an item and the total to pay. The seller sees inventory, delivery and the amount earned. The platform tracks the order and the costs of moving money. An item can be reserved before payment settles. A paid order can still require delivery or dispute review. A seller can accumulate a balance across orders before requesting a withdrawal. These distinctions are why the catalog, order history and financial statement each have a place in the product.

Trustly MM starts from a different setting. The participants already share a Discord conversation and need a common record of a deal. The bot coordinates the exchange, while the dashboard gives staff another view of its progress. A conversation can explain what the participants intended. The financial records establish which movements actually took place. The engineering work includes making those views agree when a provider sends the same notification more than once.

## 🖥️ Software that crosses the desktop boundary

FlarkFPS has two release surfaces. The storefront handles purchase and license delivery. The Windows application reads activation state and presents changes a user can make to the machine. Testing a successful checkout answers one question. Testing whether an installed build can apply a supported setting and restore the previous value answers another. A release that touches both needs evidence from both environments.

## 🌎 Publishing products in two languages

Flark Group presents a catalog whose identity and ordering carry across Portuguese and English. A translated project title needs a matching description, accessible image text and action. Some entries lead to a product, while others have a contact action. The personal portfolio has a different editorial job. Its project previews explain a contribution, and its contact interaction leaves the visitor in control of copying and sending an introduction.

The profile is the shortest route into that body of work. Readers interested in settlement and reconciliation can start with Trokano or Trustly MM. Readers interested in the boundary between web and native applications can start with FlarkFPS. For publishing and accessibility, the two portfolios show how a small static surface can still require careful language, navigation and keyboard behavior.

## 🛠️ Technical focus

I work with TypeScript and Node.js for web products and APIs, Python for services and automation, Swift for native tooling, and PostgreSQL for persistent data.

### 🧱 Different systems, different sources of truth

In a marketplace, a payment notification, an inventory reservation, and a withdrawal each describe a different event. In a desktop application, a local account file and a server-issued license have different responsibilities. In a static portfolio, the source of truth is the content that generates the pages. These distinctions explain why the projects use different architectures even when they share a language or framework.

### 🗺️ An engineering reading guide

| Interest | Project to explore | Concrete question to follow |
| --- | --- | --- |
| Money represented as integer cents | Trokano | How does the order quote distinguish the seller's commission from the buyer's service fee? |
| Durable financial state across interfaces | Trustly MM | Which process owns writes when the bot and dashboard display the same deal? |
| Moving from checkout to a native application | FlarkFPS | Which record ties fulfillment to entitlement, and which checks need a Windows machine? |
| A complete site without a running backend | Nordic portfolio | Which pages are generated at build time, and which interactions are added in the browser? |
| Bilingual product publishing | Flark Group | How do a stable slug, local preview and two sets of copy produce one coherent catalog? |

The project documentation follows these questions down to specific inputs and outcomes. A fee example is useful when its inputs can be reproduced. A native application claim needs the relevant operating system. A static page can be inspected from its generated files. Keeping those boundaries visible makes it easier to decide which repository holds the evidence for a given question.

### 📖 About this repository

GitHub renders this Markdown file as my profile. The project names above identify the products and the engineering problems they illustrate. Edits here change the profile presentation; the implementation, tests, and operating instructions belong to the individual repositories. Preview the rendered Markdown when changing the product table, particularly on narrow screens.
