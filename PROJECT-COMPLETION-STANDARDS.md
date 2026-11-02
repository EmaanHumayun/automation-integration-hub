# Project Completion Standards

This document defines the verification rubric and completion criteria required to advance a project from planned to completed status.

---

## Completion Criteria Rubric

A project is marked **Completed** only when all five criteria below are satisfied:

| Criteria | Requirement | Verification Method |
| :--- | :--- | :--- |
| **1. Specification & Requirements** | All 20 specification sections and functional requirements complete | Review `PROJECT-SPECIFICATION.md` |
| **2. Guided Practical Labs** | Minimum 3 practical labs executed with documented terminal evidence | Verify logs in `reports/` |
| **3. Independent Assignment** | Assessment challenge implemented and verified against rubric | Review `assignments/` solution |
| **4. Runnable Source Code** | Working triggers, services, and actions with zero hardcoded credentials | Code review in `src/` |
| **5. Automated Test Suite** | Unit and integration test suite passing with documented output | Run `npm test` or `pytest` |

---

## Authentic Status Definitions

- **Planned**: Project specification, architecture, requirements, labs, and directory scaffolding are established. Implementation has not yet begun.
- **In Progress**: Active code development, lab exercises, or testing underway.
- **Testing**: Implementation complete; automated test suites and validation in progress.
- **Completed**: All rubric requirements verified with working code and passing tests.
- **Deployed**: Application running in a staging or production containerized environment.
