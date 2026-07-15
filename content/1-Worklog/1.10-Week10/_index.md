---
title: "Week 10 Worklog"
date: 2026-06-26
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Light reference learning only (look things up when needed), focused on finishing the API/Frontend and integrating all layers of the Genzite Project.
* Build a complete REST API layer for CMS and AI generation, and connect it to the React/TypeScript Frontend.
* Integrate Networking (VPC/Security Group) and run full end-to-end integration tests across the whole system.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                                                                                                                                                                                               | Start Date | End Date   | References                                                                                                                                                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mon | **GENZITE:** <br> - Build/finalize the API layer (REST API NestJS controllers) <br> - Fully define endpoints for CMS + AI generation (GET/POST/PUT/DELETE) <br> **QUICK REFERENCE (as needed):** <br> - API design best practices – 10-15 min <br> **LABS & NOTES:** <br> - Reference: 000022.awsstudygroup.com                                                    | 22/06/2026 | 22/06/2026 | [000022.awsstudygroup.com](https://000022.awsstudygroup.com)                                                                                                               |
| Tue | **GENZITE:** <br> - Finalize the Frontend (React/TypeScript) calling the API <br> - Connect Frontend ↔ API layer (CMS editor + AI generation UI) <br> **LABS & NOTES:** <br> - Reference: cloudjourney.awsstudygroup.com                                                                                                                                           | 23/06/2026 | 23/06/2026 | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com)                                                                                                   |
| Wed | **GENZITE:** <br> - Integrate Networking (VPC/Security Group) to secure the entire system <br> - Review Security Groups and IAM Roles across the whole architecture (ai-service, backend, database) <br> **LIGHT REFERENCE LEARNING:** <br> - Review VPC Endpoint for internal services – 20 min <br> **LABS & NOTES:** <br> - Reference: 000003.awsstudygroup.com | 24/06/2026 | 24/06/2026 | [000003.awsstudygroup.com](https://000003.awsstudygroup.com)                                                                                                               |
| Thu | **GENZITE:** <br> - Run comprehensive integration testing across the whole system <br> - Test key use-cases: generate an AI website, edit CMS content, publish <br> - Record and fix any bugs found <br> **LABS & NOTES:** <br> - Reference: cloudjourney.awsstudygroup.com                                                                                        | 25/06/2026 | 25/06/2026 | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com)                                                                                                   |
| Fri | **PRACTICE & LEARN MORE:** <br> - Review overall Genzite progress (Backend+Storage+API+Frontend) <br> - Write the Week 10 Worklog <br> - Update the Genzite Proposal (near complete) <br> - Start drafting the Workshop Documentation (FCJ Hugo template) <br> **LABS & NOTES:** <br> - github.com/thienluhoan/fcj-workshop-template <br> - Write Week 10 Worklog  | 26/06/2026 | 26/06/2026 | [github.com/thienluhoan/fcj-workshop-template](https://github.com/thienluhoan/fcj-workshop-template) <br> [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project) |


### Week 10 Achievements:

* **API Layer:** API endpoints covering all core functionality, successfully tested via Postman/curl.
* **Frontend Integration:** Frontend displaying data and calling the API successfully, basic UI covering all core functionality.
* **Networking & Security:** All traffic correctly routed through the designated subnets/Security Groups, no clear access control gaps.
* **Integration Testing:** System running stably end-to-end, key bugs fixed.
* **Summary:** Genzite Project ~75% complete. Genzite Proposal 85%. Workshop documentation draft 20%. Week 10 Worklog completed.