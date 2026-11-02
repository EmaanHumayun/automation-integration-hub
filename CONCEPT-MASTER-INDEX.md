# Concept Master Index

This master index maps all fundamental, intermediate, advanced, and professional automation concepts to the projects in which they are introduced and applied.

---

## 1. Automation Fundamentals

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **Triggers** | Event-based mechanisms initiating workflow execution | Project 01 | Projects 01 - 20 |
| **Actions** | Discrete functional operations executed in response to a trigger | Project 01 | Projects 01 - 20 |
| **Conditions** | Logical branching based on payload evaluation | Project 01 | Projects 02, 03, 06, 09, 12 |
| **Scheduling** | Time-based cron execution for recurring tasks | Project 02 | Projects 04, 08, 10, 14, 18 |
| **Workflow Execution** | Managing lifecycle and execution context of a workflow | Project 01 | Projects 01 - 20 |
| **Variables & Context** | Scoped state and environment variable management | Project 01 | Projects 01 - 20 |
| **Data Mapping** | Transforming input schemas to required destination shapes | Project 01 | Projects 02, 05, 06, 11, 14 |
| **Loops & Iteration** | Sequential and parallel batch processing of collections | Project 02 | Projects 04, 05, 10, 14 |
| **Error Handling** | Structured capture, logging, and recovery from runtime faults | Project 01 | Projects 01 - 20 |
| **Input Validation** | Schema verification ensuring payloads conform to contracts | Project 01 | Projects 03, 06, 07, 11, 15 |

---

## 2. API and Integration Engineering

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **REST APIs** | Consuming and exposing standard HTTP RESTful interfaces | Project 01 | Projects 01 - 20 |
| **JSON Schemas** | Contract definition and validation for payloads | Project 01 | Projects 03, 05, 11, 15 |
| **API Keys & Basic Auth** | Secret-based authentication mechanisms | Project 01 | Projects 02, 04, 05 |
| **OAuth 2.0 Grant** | User authorization code flow and refresh token rotation | Project 02 | Projects 06, 08, 11 |
| **Pagination Handling** | Navigating offset, cursor, and keyset-based paginated endpoints | Project 05 | Projects 06, 08, 10, 14 |
| **Rate Limiting & Backoff** | Token bucket pacing and exponential backoff with jitter | Project 05 | Projects 06, 07, 11, 20 |
| **Webhooks Ingest** | Asynchronous HTTP callback reception and processing | Project 01 | Projects 03, 06, 07, 09, 13, 17 |
| **HMAC Verification** | Cryptographic verification of webhook payload authenticity | Project 01 | Projects 07, 10, 13, 17 |
| **Idempotency Keys** | Ensuring identical operations produce consistent results safely | Project 07 | Projects 10, 12, 13, 20 |

---

## 3. Workflow Architecture and Distributed Systems

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **Sequential Execution** | Deterministic pipeline of linear processing steps | Project 01 | Projects 01 - 05 |
| **Parallel Fan-Out/Fan-In** | Concurrent execution of subtasks with synchronization barriers | Project 05 | Projects 08, 12, 14, 19 |
| **Directed Acyclic Graph** | Arbitrary dependency graph execution for workflows | Project 12 | Project 12, 19 |
| **State Persistence** | Storing execution state in external databases for durability | Project 03 | Projects 06, 07, 11, 12, 20 |
| **Distributed Queues** | Asynchronous message passing via Redis / RabbitMQ | Project 06 | Projects 07, 12, 13, 16, 20 |
| **Dead-Letter Exchanges** | Capturing failed messages for inspection and re-drive | Project 13 | Projects 13, 16, 20 |
| **Compensating Transactions** | Rolling back distributed side effects upon step failure | Project 12 | Projects 12, 20 |

---

## 4. Data Engineering and ETL

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **ETL Pipelines** | Extract, Transform, Load workflows for operational data | Project 10 | Projects 14, 18 |
| **Incremental Sync** | Delta detection using high-watermark timestamps | Project 02 | Projects 10, 14 |
| **Deduplication** | Content fingerprinting and hash comparison to prevent duplicates | Project 03 | Projects 06, 14 |
| **Schema Evolution** | Handling changing field structures without breaking pipelines | Project 11 | Projects 14, 20 |
| **Data Normalization** | Unifying diverse external formats into canonical domain models | Project 05 | Projects 11, 14, 15 |

---

## 5. DevOps and Infrastructure Automation

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **Containerization** | Docker packaging for reproducible automation runtimes | Project 01 | Projects 01 - 20 |
| **Multi-Service Compose** | Orchestrating app, database, and cache dependencies locally | Project 06 | Projects 07, 12, 13, 20 |
| **CI/CD Automation** | Automating build, test, and deployment via GitHub Actions | Project 16 | Projects 17, 20 |
| **Infrastructure as Code** | Declarative cloud resource provisioning with Terraform | Project 18 | Projects 18, 20 |
| **SSH Automation** | Programmatic remote server administration and command dispatch | Project 16 | Project 16 |
| **Self-Healing Runbooks** | Automated remediation scripts triggered by observability alerts | Project 16 | Projects 16, 18 |
| **Kubernetes Deployments** | Cloud-native container orchestration with health checks | Project 20 | Project 20 |

---

## 6. AI and Multi-Agent Systems

| Concept | Description | Introduced In | Applied In |
| :--- | :--- | :--- | :--- |
| **LLM Structured Output** | Enforcing strict JSON schema returns from language models | Project 15 | Projects 15, 19 |
| **Document Entity Extraction** | Parsing semi-structured documents into relational data | Project 15 | Project 15 |
| **Multi-Agent Coordination** | Multi-agent graphs executing collaborative workflows | Project 19 | Project 19 |
| **Human-in-the-Loop** | Workflow pauses requiring authorized manual confirmation | Project 19 | Projects 19, 20 |
| **Audit Trails & Lineage** | Comprehensive tracking of automated agent decisions | Project 19 | Projects 19, 20 |
