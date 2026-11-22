# 👋 nordic

I build web applications, APIs, and databases. My work spans the interface people use, the services behind it, and the infrastructure that keeps it running.

## 🧾 Products and the problems they solve

| Project | What someone uses it for | Engineering concern |
| --- | --- | --- |
| Trokano | Buy or sell a digital item with payment held until delivery | Keeping inventory, order status, and the seller’s balance consistent |
| Trustly MM | Coordinate an escrow trade without leaving the Discord conversation | Sharing deal state between the bot, the API, and the dashboard |
| FlarkFPS | Review Windows performance settings and manage a desktop license | Preserving the original system settings and validating activation on the server |
| Flark Group | Explore the bilingual product catalog | Publishing the same catalog in Portuguese and English |

## 🛠️ Technical focus

I work with TypeScript and Node.js for web products and APIs, Python for services and automation, Swift for native tooling, and PostgreSQL for persistent data.

### 🧱 Different systems, different sources of truth

In a marketplace, a payment notification, an inventory reservation, and a withdrawal each describe a different event. In a desktop application, a local account file and a server-issued license have different responsibilities. In a static portfolio, the source of truth is the content that generates the pages. These distinctions explain why the projects use different architectures even when they share a language or framework.

### 📖 About this repository

GitHub renders this Markdown file as my profile. The project names above identify the products and the engineering problems they illustrate. Edits here change the profile presentation; the implementation, tests, and operating instructions belong to the individual repositories. Preview the rendered Markdown when changing the product table, particularly on narrow screens.
