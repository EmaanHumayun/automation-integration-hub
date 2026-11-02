# Integrations Catalog

This catalog documents external protocols, services, and platforms integrated across the 20 progressive projects.

---

## 1. Protocols and Core Interfaces

| Protocol / Standard | Purpose | Projects |
| :--- | :--- | :--- |
| **HTTP / REST** | Synchronous API communication, webhooks, and client endpoints | Projects 01 - 20 |
| **HMAC-SHA256** | Webhook payload authentication and tamper detection | Projects 01, 07, 10, 13, 17 |
| **OAuth 2.0** | Third-party user authorization and scoped token management | Projects 02, 06, 08, 11 |
| **SMTP / TLS** | Transactional email dispatch and notifications | Projects 01, 03, 10 |
| **AMQP 0-9-1** | Asynchronous message queuing and topic exchanges (RabbitMQ) | Projects 13, 16, 20 |
| **SSH / SFTP** | Secure shell remote server administration and file transfer | Project 16 |
| **OpenTelemetry** | Standardized distributed tracing and metrics emission | Projects 12, 20 |

---

## 2. Third-Party SaaS and Developer APIs

| Category | Platform / Service | Projects |
| :--- | :--- | :--- |
| **Productivity** | Google Sheets API, Google Workspace | Projects 02, 05 |
| **Communication** | Slack Webhooks, Discord Webhooks, SendGrid / Nodemailer | Projects 01, 03, 09, 16 |
| **CRM & Sales** | HubSpot CRM API, Mock CRM Endpoints | Project 06 |
| **Fintech & Billing** | Stripe Webhooks and Billing API, PayPal Mock API | Projects 07, 10 |
| **Customer Support** | Zendesk API, Intercom Mock API | Project 09 |
| **Social Media** | Meta Graph API, X API | Project 08 |
| **Developer Platforms** | GitHub REST / GraphQL API, Octokit | Project 17 |
| **AI Platforms** | OpenAI API, Google Gemini API, Anthropic API | Projects 15, 19 |
| **Cloud Providers** | AWS (EC2, S3, Lambda, CloudWatch, IAM) | Projects 04, 18, 20 |

---

## 3. Databases, Caches, and Message Brokers

| System | Role in Ecosystem | Projects |
| :--- | :--- | :--- |
| **SQLite** | Embedded relational storage for lightweight local services | Projects 03, 05 |
| **PostgreSQL** | Primary relational database for transactions, tickets, and state | Projects 07, 10, 12, 14, 20 |
| **Redis** | In-memory cache, rate limiter state, and BullMQ job storage | Projects 06, 07, 11, 13, 19 |
| **RabbitMQ** | Message broker for decoupled, resilient event consumption | Projects 13, 16, 20 |
| **MinIO / AWS S3** | S3-compatible object storage for file archiving and logs | Projects 04, 08, 18 |
