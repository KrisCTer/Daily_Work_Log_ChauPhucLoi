---
title: "Week 11 Worklog"
date: 2026-07-03
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Light reference learning only (only when stuck), focused on finalizing the Genzite Project: Monitoring, basic security (WAF/Secrets Manager/Security Hub), and Workshop Documentation.
* Add advanced Monitoring (CloudWatch Dashboard + Alarms) and review basic security (IAM least privilege, KMS encryption, Security Hub).
* Optimize costs, write the bilingual Workshop Documentation, and draft the Self-evaluation, bringing Genzite to ~95% complete.

### Tasks to be implemented this week:
| Day | Task                                                                                                                                                                                                                                                                                                                                                                                                          | Start Date | End Date   | References                                                                                                                                                                 |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mon | **REFERENCE LEARNING (as needed):** <br> - AWS WAF: web ACL, rules, managed rule groups <br> **GENZITE:** <br> - Add Monitoring to the system – advanced CloudWatch Dashboard + Alarms <br> - Track key metrics (CPU, error rate, BullMQ queue depth, Gemini API latency) <br> - Consider attaching WAF to the ALB in front of the Frontend <br> **LABS & NOTES:** <br> - Reference: 000008.awsstudygroup.com | 29/06/2026 | 29/06/2026 | [000008.awsstudygroup.com](https://000008.awsstudygroup.com)                                                                                                               |
| Tue | **REFERENCE LEARNING (as needed):** <br> - Security Hub findings, GuardDuty threat detection <br> **GENZITE:** <br> - Basic security review – IAM least privilege, encrypt sensitive data (KMS) <br> - Re-check Security Hub/Permission Boundary applied since Module 5 <br> **LABS & NOTES:** <br> - Reference: 000033.awsstudygroup.com, 000018.awsstudygroup.com                                           | 30/06/2026 | 30/06/2026 | [000033.awsstudygroup.com](https://000033.awsstudygroup.com) <br> [000018.awsstudygroup.com](https://000018.awsstudygroup.com)                                             |
| Wed | **GENZITE:** <br> - Cost optimization – review running resources (ECS task, RDS, ElastiCache), delete/resize unneeded resources <br> - Check Cost Explorer, ensure spending stays within budget <br> **LIGHT REFERENCE LEARNING:** <br> - Review Cost Optimization (Savings Plans, Right-sizing) – 20 min <br> **LABS & NOTES:** <br> - Reference: 000064.awsstudygroup.com                                   | 01/07/2026 | 01/07/2026 | [000064.awsstudygroup.com](https://000064.awsstudygroup.com) <br> [rules.fcjuni.com](https://rules.fcjuni.com)                                                             |
| Thu | **PRACTICE & LEARN MORE:** <br> - Write the Workshop Documentation (bilingual VI/EN) using the FCJ template <br> - Add Genzite architecture diagrams, code snippets (NestJS modules, Prisma transaction fix, BullMQ flow), and detailed deployment steps <br> **GENZITE:** <br> - Final end-to-end testing, capture demo screenshots <br> **LABS & NOTES:** <br> - workshop-sample.fcjuni.com                 | 02/07/2026 | 02/07/2026 | [workshop-sample.fcjuni.com](https://workshop-sample.fcjuni.com) <br> [github.com/thienluhoan/fcj-workshop-template](https://github.com/thienluhoan/fcj-workshop-template) |
| Fri | **PRACTICE & LEARN MORE:** <br> - Finalize the Workshop Documentation to 90% <br> - Write the Week 11 Worklog <br> - Write the Self-evaluation (8 FCJ criteria) – draft <br> - Genzite Project overall progress ~95% <br> **LABS & NOTES:** <br> - Write Week 11 Worklog                                                                                                                                      | 03/07/2026 | 03/07/2026 | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)                                                                                                           |


### Week 11 Achievements:

* **Monitoring:** Full CloudWatch Dashboard monitoring the Genzite Project, alarms triggering on errors/high load, and clear understanding of how WAF blocks malicious requests.
* **Security:** Basic security checklist completed, sensitive data encrypted (KMS) where needed, Security Hub scan no longer showing critical findings.
* **Cost Optimization:** Genzite costs kept under control, unneeded resources cleaned up.
* **Workshop Documentation:** Documentation 70% complete after Thursday (VI+EN), full set of demo screenshots for all key steps; finalized to 90% by Friday.
* **Summary:** Self-evaluation draft completed. **Genzite Project overall progress ~95% complete**. Week 11 Worklog completed.