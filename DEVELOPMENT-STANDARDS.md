# Development Standards

This document establishes the coding conventions, directory structure, error handling policies, and testing guidelines for all automation projects.

---

## 1. Directory Structure Standard

Every project directory must strictly follow this internal structure:

```
project-name/
|-- README.md                    # Project overview, setup, and execution instructions
|-- PROJECT-SPECIFICATION.md     # 20-point comprehensive engineering specification
|-- REQUIREMENTS.md              # Functional, non-functional, and security requirements
|-- IMPLEMENTATION-ROADMAP.md    # Phased milestones and technical checklist
|-- CHANGELOG.md                 # Project version history and change record
|-- .gitignore                   # Ignore node_modules, .env, *.log, build artifacts
|-- .env.example                 # Sanitized environment variable template
|
|-- labs/                        # Guided progressive practical labs
|   |-- lab-01-setup-and-prerequisites.md
|   |-- lab-02-core-workflow-implementation.md
|   `-- lab-03-validation-and-testing.md
|
|-- assignments/                 # Independent assessment challenges
|   `-- assignment-01-core-enhancement.md
|
|-- workflows/                   # Sanitized workflow definitions and templates
|   |-- development/
|   |-- production/
|   `-- examples/
|
|-- src/                         # Application source code
|   |-- config/                  # Environment loading and configuration
|   |-- integrations/            # Third-party API client modules
|   |-- triggers/                # Webhook listeners, cron jobs, event consumers
|   |-- actions/                 # Outbound operations (email, database, API calls)
|   |-- services/                # Business logic and transformation pipelines
|   `-- utils/                   # Shared helpers, validators, loggers
|
|-- docs/                        # Technical documentation
|   |-- architecture/
|   |-- workflows/
|   |-- APIs/
|   |-- webhooks/
|   |-- database/
|   `-- decisions/
|
|-- tests/                       # Automated test suites
|-- examples/                    # Sample inputs, mock payloads, test fixtures
|-- reports/                     # Lab execution outputs, test runs, audit evidence
`-- deployment/                  # Dockerfile, docker-compose.yml, k8s manifests
```

---

## 2. Environment Configuration & Secret Isolation

- Never hardcode API keys, database credentials, or tokens in source code.
- Always read configurations via `process.env` (Node.js) or `os.environ` (Python) through a centralized config module.
- Always provide a clean, updated `.env.example` with descriptive placeholder keys.

---

## 3. Error Handling and Logging Standard

- All external API calls must be wrapped in structured try-catch blocks with defined timeout limits.
- Log messages must be emitted as structured JSON objects containing:
  - `timestamp`: ISO 8601 string
  - `level`: `INFO`, `WARN`, `ERROR`, or `DEBUG`
  - `trace_id` / `correlation_id`: Unique identifier tracking the execution lifecycle
  - `context`: Workflow step, external service name, and execution duration
