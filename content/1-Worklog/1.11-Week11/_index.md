---
title: "Week 11 Worklog"
date: 2026-07-03
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Finalize the admin UI and Canvas Builder with real generation metrics, persisting action history to the database.
* Integrate Cognito login and image upload via the Media service (S3), and standardize the UI architecture to English.
* Remove the unneeded commerce-service, set up production CI/CD, and enforce strict TypeScript across the monorepo.

### Tasks completed this week:
| Day | Task | Start Date | End Date | References |
| --- | ---- | ---------- | -------- | ---------- |
| Mon | **Admin UI:** <br> - Adjusted the admin-identity-profile-notification UI | 29/06/2026 | 29/06/2026 |  |
| Tue | **Canvas & Builder Finalization:** <br> - Continued the Canvas refactor by persisting real generation metrics, dynamic action history, removing mock descriptions, and storing prompts in the DB <br> - Updated the Canvas Builder UI and improved the Login/Home/Dashboard layout <br> - Resolved EditViewer.tsx merge conflicts and enforced an English UI modular architecture | 30/06/2026 | 30/06/2026 |  |
| Wed | **Cognito & S3 Integration:** <br> - Implemented Cognito login, image upload through the Media service, profile picture editing, and login bug fixes | 01/07/2026 | 01/07/2026 |  |
| Thu | **Cognito Finalization & i18n Standardization:** <br> - Resolved EditViewer.tsx conflicts, introduced a glowing prompt-improvement UI with fallback timeouts, implemented the Component-Driven Generation architecture, refined CanvasWorkspace and real-time View Details metrics, and added a deep recursive regex scanner for nested image URLs in widgets <br> - Translated hardcoded Vietnamese strings to English and cleaned up dead AI files <br> - Finalized Cognito + S3 integration, fixed the default VIEWER role on SSO registration, adjusted the assigned UI sections, and fixed notification/change-password issues | 02/07/2026 | 02/07/2026 |  |
| Fri | **Cleanup & Production CI/CD:** <br> - Removed the unused commerce-service, cleaned up related dead code across frontend and backend, updated architecture docs to the finalized 6-service model, created a centralized infra/Dockerfile.prod optimized for pnpm workspaces, implemented GitHub Actions for ECS deployment (backend) and Vercel deployment (frontend), and updated the Production Deployment guide <br> - Enforced strict TypeScript rules monorepo-wide, created shared RequestWithUser/AuthUser interfaces, and fixed implicit-any issues in ai.consumer.ts and site-generator.service.ts | 03/07/2026 | 03/07/2026 |  |

### Week 11 Achievements:

* **Canvas Builder Finalized:** Real-time generation metrics were persisted correctly, dynamic action history replaced mock data, and prompts were stored in the DB for traceability.
* **Cognito Authentication & Media:** Login via Amazon Cognito worked stably, profile picture upload/editing through the Media service (S3) worked correctly, and the default VIEWER role was correctly applied on SSO registration.
* **Codebase Standardization:** All hardcoded Vietnamese strings were translated to English, and the UI architecture was modularized according to the English standard.
* **Simplified Architecture:** The unused commerce-service was fully removed, and the architecture docs were updated to the correct 6-service model.
* **CI/CD & Code Quality:** Automated CI/CD was successfully set up (GitHub Actions for backend ECS deployment and Vercel frontend deployment), the codebase now meets strict TypeScript standards (including noImplicitAny), and a production Dockerfile optimized for pnpm workspaces was created.