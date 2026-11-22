# 👋 nordic

I build web applications, APIs, and databases. My work spans the interface people use, the services behind it, and the infrastructure that keeps it running.

## 🧭 Project handbook

### 🧾 Products and the problems they solve

| Project | What someone uses it for | Engineering concern |
| --- | --- | --- |
| Trokano | Buy or sell a digital item with payment held until delivery | Keeping inventory, order status, and the seller’s balance consistent |
| Trustly MM | Coordinate an escrow trade without leaving the Discord conversation | Sharing deal state between the bot, the API, and the dashboard |
| FlarkFPS | Review Windows performance settings and manage a desktop license | Preserving the original system settings and validating activation on the server |
| Flark Group | Explore the bilingual product catalog | Publishing the same catalog in Portuguese and English |

### 🛍️ What a marketplace order involves

Trokano connects three perspectives on one purchase. A buyer sees an item and the total to pay. The seller sees inventory, delivery and the amount earned. The platform tracks the order and the costs of moving money. An item can be reserved before payment settles. A paid order can still require delivery or dispute review. A seller can accumulate a balance across orders before requesting a withdrawal. These distinctions are why the catalog, order history and financial statement each have a place in the product.

Trustly MM starts from a different setting. The participants already share a Discord conversation and need a common record of a deal. The bot coordinates the exchange, while the dashboard gives staff another view of its progress. A conversation can explain what the participants intended. The financial records establish which movements actually took place. The engineering work includes making those views agree when a provider sends the same notification more than once.

### 🖥️ Software that crosses the desktop boundary

FlarkFPS has two release surfaces. The storefront handles purchase and license delivery. The Windows application reads activation state and presents changes a user can make to the machine. Testing a successful checkout answers one question. Testing whether an installed build can apply a supported setting and restore the previous value answers another. A release that touches both needs evidence from both environments.

### 🌎 Publishing products in two languages

Flark Group presents a catalog whose identity and ordering carry across Portuguese and English. A translated project title needs a matching description, accessible image text and action. Some entries lead to a product, while others have a contact action. The personal portfolio has a different editorial job. Its project previews explain a contribution, and its contact interaction leaves the visitor in control of copying and sending an introduction.

The profile is the shortest route into that body of work. Readers interested in settlement and reconciliation can start with Trokano or Trustly MM. Readers interested in the boundary between web and native applications can start with FlarkFPS. For publishing and accessibility, the two portfolios show how a small static surface can still require careful language, navigation and keyboard behavior.

## 📚 Field reference

### 🧭 Choose a project by the decision it helps someone make

| Reader's question | Project | What to look for in its documentation |
| --- | --- | --- |
| What happens to the last unit when two people try to buy it? | Trokano | How a catalog option, inventory reservation and historical order item refer to one another. |
| How do two participants agree to the same trade terms? | Trustly MM | How the buyer and seller confirm a deal, and what happens to confirmation if the terms change. |
| What does someone receive after buying desktop software? | FlarkFPS | The handoff from a paid order to a license, then from a license to an installed session. |
| How do people find the right product in either language? | Flark Group | How one catalog supplies the project identity, preview, description and action in each language. |

A useful way to read the projects is to follow a single object. In Trokano that can be an option purchased at a particular price. The current listing can change while the receipt still has to describe the original purchase. In Trustly MM it can be a negotiation ID shared between the conversation and the transaction record. In FlarkFPS it can be the license attached to a fulfilled order. The identifiers are meaningful because a reader can follow them across time, across screens or between applications.

### 🧪 What different kinds of evidence establish

Consider the claim that someone can buy a product and use it on Windows. A working storefront can show the offer. A purchase fixture can establish how fulfillment reacts to a payment. Opening the desktop application can show the sign-in experience. An installed-device exercise can show how a particular Windows configuration behaves. Those observations complement one another. Recording which one was actually made is part of making the documentation useful to the next person evaluating the project.

A bilingual page has a different evidence trail. View the generated document with scripts disabled to inspect the core reading experience. Use the interactive page to examine filtering, navigation and clipboard feedback. Then inspect the narrow layout to see whether a translated label still fits next to its control. A text comparison between two locales can catch missing content, while a rendered review can reveal a problem that neither the content file nor a build log makes visible.

### 📖 Reading this profile as a project index

The shared theme is software whose users need to understand an outcome: a payment settled, a role confirmed, an application activated or a project found. Start with the product whose outcome interests you. Its own README explains the participants, representative inputs, boundaries between components and limits of its checks. This profile provides the cross-project context. Exact commands, platform requirements and release instructions belong to the individual project where they can be maintained alongside the implementation.

### 🗂️ Three questions before publishing a case study

**What did the person using the product need to decide?** A buyer deciding whether a purchase is complete needs a different explanation from staff reconciling a withdrawal. Describing those roles gives context to the engineering work and helps a reader choose the relevant project.

**Which parts had to agree?** A checkout record can agree with the payment provider while the seller is still waiting for delivery or release. A license can exist before a desktop session starts. A shared catalog entry can be correct while one localized action label is missing. Naming the two observations makes a case study more informative than listing the technologies alone.

**How could someone tell the work succeeded?** Use an outcome a reader can understand: a receipt retains the original price, both parties see the same agreed terms, a licensed session opens, or both localized pages lead to the intended action. When more evidence would be needed to establish a production result, describe the engineering question at the level the available evidence supports.

<a id="-technical-focus"></a>

## 🛠️ Technical details

I work with TypeScript and Node.js for web products and APIs, Python for services and automation, Swift for native tooling, and PostgreSQL for persistent data.

### 📝 Maintaining a public profile entry

Decide which claim an entry makes before changing its wording. A user-facing description can explain what problem the product solves. A technical description can name the component responsible for a particular outcome. An experience statement needs evidence for the individual's contribution. Release status and current infrastructure are time-sensitive. Verify them before publishing a claim that a service is available or that a feature is in production.

| Proposed change | Evidence to use | Detail suitable for the profile |
| --- | --- | --- |
| Add a product | Its established public identity and a verified use case | One sentence explaining what a person can do. |
| Name a technology | The project manifest or direct implementation evidence | Which part uses it and why it is relevant to the example. |
| Describe a design contribution | The case study and its stated scope | Distinguish a delivered interface from a visual study. |
| Update a maintenance claim | Current project documentation and dated evidence | Explain the engineering concern without exposing internal deployment details. |

The profile itself has a single Markdown rendering target. Review long table cells on a narrow viewport, meaningful heading order for keyboard and screen-reader navigation, and project names in plain text. A standalone reader should understand each row without access to private source or production accounts. [Repository conventions](AGENTS.md)

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
