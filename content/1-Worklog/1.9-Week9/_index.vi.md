---
title: "Worklog Tuần 9"
date: 2026-06-19
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---



### Mục tiêu tuần 9:

* Học nhẹ (tham khảo khi cần), tập trung xây dựng Backend layer (NestJS modules) và Storage layer (S3) cho Genzite Project.
* Deploy Backend lên ECS Fargate với IAM Role đúng phạm vi cho S3/RDS/Secrets Manager.
* Kết nối Backend ↔ Database ↔ S3 thành luồng end-to-end hoàn chỉnh, có test case cơ bản.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ | --------------- | ------------------------------------------------------------------------- |
| 2   | **GENZITE:** <br> - Triển khai/hoàn thiện Backend layer (NestJS modular monolith) cho các domain CMS chính <br> - Viết/refactor logic xử lý CRUD cho dynamic CMS (JSONB storage theo guardrail đã chốt) <br> **HỌC NHẸ (tham khảo khi cần):** <br> - EC2/ECS service scaling – 20-30 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: cloudjourney.awsstudygroup.com | 15/06/2026   | 15/06/2026      | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/) |
| 3   | **GENZITE:** <br> - Deploy Backend (NestJS modules) lên AWS (ECS Fargate) <br> - Cấu hình IAM Role cho task ECS truy cập S3/RDS/Secrets Manager <br> **HỌC NHẸ:** <br> - Ôn IAM Role cho ECS task – 20 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000048.awsstudygroup.com                                                                                     | 16/06/2026   | 16/06/2026      | [000048.awsstudygroup.com](https://000048.awsstudygroup.com/)             |
| 4   | **GENZITE:** <br> - Triển khai Storage layer – S3 bucket cho media/file của dự án (ảnh AI generate, assets website) <br> - Cấu hình bucket policy, lifecycle rule <br> **HỌC NHẸ:** <br> - Ôn S3 storage class & lifecycle – 20 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000057.awsstudygroup.com                                                            | 17/06/2026   | 17/06/2026      | [000057.awsstudygroup.com](https://000057.awsstudygroup.com/)             |
| 5   | **GENZITE:** <br> - Kết nối Backend ↔ Database (Prisma/RDS) ↔ S3 thành luồng end-to-end <br> - Test toàn bộ flow: request → backend → database/S3 → response <br> - Viết test case cơ bản (happy path + 1-2 edge case) cho generation flow + CMS flow <br> **LAB & GHI CHÚ:** <br> - Tham khảo: cloudjourney.awsstudygroup.com                                     | 18/06/2026   | 18/06/2026      | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/) |
| 6   | **THỰC HÀNH & HỌC THÊM:** <br> - Review & debug Backend/Storage layer <br> - Viết Worklog Tuần 9 <br> - Cập nhật Proposal Capstone (chi tiết Backend + Storage) <br> - Chụp ảnh demo tiến độ tuần 9 <br> **LAB & GHI CHÚ:** <br> - Viết Worklog Tuần 9                                                                                                             | 19/06/2026   | 19/06/2026      | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)          |


### Kết quả đạt được tuần 9:

* **Backend Layer:** Backend service chạy được local/dev, logic CRUD CMS hoạt động đúng theo guardrail JSONB-only.
* **Deploy Backend:** Backend deploy thành công trên AWS (ECS Fargate), IAM Role áp dụng đúng nguyên tắc least privilege.
* **Storage Layer:** S3 bucket hoạt động đúng phân quyền, lifecycle policy đã set (tối ưu chi phí).
* **Tích hợp End-to-End:** Flow end-to-end Backend+DB+S3 hoạt động, test case pass.
* **Tổng kết:** Backend + Storage layer ổn định, demo được. Proposal Capstone đạt 60%. Hoàn thành Worklog Tuần 9.