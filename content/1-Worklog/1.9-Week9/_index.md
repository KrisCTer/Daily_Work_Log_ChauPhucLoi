---
title: "Week 9 Worklog"
date: 2026-06-19
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Light reference learning only (as needed), focused on building the Backend layer (NestJS modules) and Storage layer (S3) for the Genzite Project.
* Deploy the Backend to ECS Fargate with a properly scoped IAM Role for S3/RDS/Secrets Manager access.
* Connect Backend ↔ Database ↔ S3 into a complete end-to-end flow with basic test coverage.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                                                                                                                                                                                                    | Start Date | End Date   | References                                                               |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ------------------------------------------------------------------------ |
| Mon | **GENZITE:** <br> - Build/finalize the Backend layer (NestJS modular monolith) for the core CMS domains <br> - Write/refactor CRUD logic for the dynamic CMS (JSONB storage per the agreed guardrail) <br> **LIGHT REFERENCE LEARNING (as needed):** <br> - EC2/ECS service scaling – 20-30 min <br> **LABS & NOTES:** <br> - Reference: cloudjourney.awsstudygroup.com | 15/06/2026 | 15/06/2026 | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com) |
| Tue | **GENZITE:** <br> - Deploy the Backend (NestJS modules) to AWS (ECS Fargate) <br> - Configure the IAM Role for the ECS task to access S3/RDS/Secrets Manager <br> **LIGHT REFERENCE LEARNING:** <br> - Review IAM Role for ECS tasks – 20 min <br> **LABS & NOTES:** <br> - Reference: 000048.awsstudygroup.com                                                         | 16/06/2026 | 16/06/2026 | [000048.awsstudygroup.com](https://000048.awsstudygroup.com)             |
| Wed | **GENZITE:** <br> - Deploy the Storage layer – an S3 bucket for the project's media/files (AI-generated images, website assets) <br> - Configure bucket policy and lifecycle rules <br> **LIGHT REFERENCE LEARNING:** <br> - Review S3 storage classes & lifecycle – 20 min <br> **LABS & NOTES:** <br> - Reference: 000057.awsstudygroup.com                           | 17/06/2026 | 17/06/2026 | [000057.awsstudygroup.com](https://000057.awsstudygroup.com)             |
| Thu | **GENZITE:** <br> - Connect Backend ↔ Database (Prisma/RDS) ↔ S3 into an end-to-end flow <br> - Test the full flow: request → backend → database/S3 → response <br> - Write basic test cases (happy path + 1-2 edge cases) for the generation flow and the CMS flow <br> **LABS & NOTES:** <br> - Reference: cloudjourney.awsstudygroup.com                             | 18/06/2026 | 18/06/2026 | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com) |
| Fri | **PRACTICE & LEARN MORE:** <br> - Review & debug the Backend/Storage layer <br> - Write the Week 9 Worklog <br> - Update the Capstone Proposal (Backend + Storage details) <br> - Capture demo screenshots of Week 9 progress <br> **LABS & NOTES:** <br> - Write Week 9 Worklog                                                                                        | 19/06/2026 | 19/06/2026 | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)         |


### Week 9 Achievements:

* **Backend Layer:** Backend service running locally/dev, CMS CRUD logic working correctly according to the JSONB-only guardrail.
* **Backend Deployment:** Backend successfully deployed on AWS (ECS Fargate), IAM Role correctly applying the least-privilege principle.
* **Storage Layer:** S3 bucket working with correct permissions, lifecycle policy set for cost optimization.
* **End-to-End Integration:** Backend + Database + S3 end-to-end flow working correctly, test cases passing.
* **Summary:** Backend + Storage layer stable and demo-ready. Capstone Proposal at 60%. Week 9 Worklog completed.