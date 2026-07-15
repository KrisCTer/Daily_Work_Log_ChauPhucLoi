---
title: "Worklog Tuần 11"
date: 2026-07-03
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---



### Mục tiêu tuần 11:

* Học nhẹ (chỉ khi gặp vướng mắc), tập trung hoàn thiện Genzite Project: Monitoring, bảo mật cơ bản (WAF/Secrets Manager/Security Hub), Workshop Documentation.
* Thêm Monitoring nâng cao (CloudWatch Dashboard + Alarm) và rà soát bảo mật cơ bản (IAM least privilege, mã hoá KMS, Security Hub).
* Tối ưu chi phí, viết Workshop Documentation song ngữ, và draft Self-evaluation, đưa Genzite lên ~95% hoàn thành.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                                                  | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                              |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ | --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2   | **HỌC THÊM (tham khảo):** <br> - AWS WAF: web ACL, rules, managed rule groups <br> **GENZITE:** <br> - Thêm Monitoring cho hệ thống – CloudWatch Dashboard + Alarm nâng cao <br> - Theo dõi metrics chính (CPU, error rate, BullMQ queue depth, Gemini API latency) <br> - Cân nhắc gắn WAF vào ALB phía trước Frontend <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000008.awsstudygroup.com | 29/06/2026   | 29/06/2026      | [000008.awsstudygroup.com](https://000008.awsstudygroup.com/)                                                                                                               |
| 3   | **HỌC THÊM (tham khảo):** <br> - Security Hub findings, GuardDuty threat detection <br> **GENZITE:** <br> - Rà soát bảo mật cơ bản – IAM least privilege, mã hoá dữ liệu nhạy cảm (KMS) <br> - Kiểm tra lại Security Hub/Permission Boundary đã áp dụng từ Module 5 <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000033.awsstudygroup.com, 000018.awsstudygroup.com                           | 30/06/2026   | 30/06/2026      | [000033.awsstudygroup.com](https://000033.awsstudygroup.com/) <br> [000018.awsstudygroup.com](https://000018.awsstudygroup.com/)                                            |
| 4   | **GENZITE:** <br> - Tối ưu chi phí – rà soát resource đang chạy (ECS task, RDS, ElastiCache), xoá/resize resource không cần <br> - Kiểm tra Cost Explorer, đảm bảo trong budget <br> **HỌC NHẸ:** <br> - Ôn Cost Optimization (Savings Plans, Right-sizing) – 20 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000064.awsstudygroup.com                                                   | 01/07/2026   | 01/07/2026      | [000064.awsstudygroup.com](https://000064.awsstudygroup.com/) <br> [rules.fcjuni.com](https://rules.fcjuni.com/)                                                            |
| 5   | **THỰC HÀNH & HỌC THÊM:** <br> - Viết Workshop Documentation (song ngữ VI/EN) theo FCJ template <br> - Bổ sung sơ đồ kiến trúc Genzite, code snippet (NestJS modules, Prisma transaction fix, BullMQ flow), bước triển khai chi tiết <br> **GENZITE:** <br> - Test end-to-end lần cuối, chụp ảnh demo <br> **LAB & GHI CHÚ:** <br> - workshop-sample.fcjuni.com                            | 02/07/2026   | 02/07/2026      | [workshop-sample.fcjuni.com](https://workshop-sample.fcjuni.com/) <br> [github.com/thienluhoan/fcj-workshop-template](https://github.com/thienluhoan/fcj-workshop-template) |
| 6   | **THỰC HÀNH & HỌC THÊM:** <br> - Hoàn thiện Workshop Documentation lên 90% <br> - Viết Worklog Tuần 11 <br> - Viết Self-evaluation (8 tiêu chí FCJ) – bản draft <br> - Genzite Project tổng tiến độ ~95% <br> **LAB & GHI CHÚ:** <br> - Viết Worklog Tuần 11                                                                                                                               | 03/07/2026   | 03/07/2026      | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)                                                                                                            |


### Kết quả đạt được tuần 11:

* **Monitoring:** Dashboard CloudWatch giám sát Genzite Project đầy đủ, alarm cảnh báo khi có lỗi/tải cao, hiểu cách WAF chặn request độc hại.
* **Bảo mật:** Checklist bảo mật cơ bản hoàn thành, dữ liệu nhạy cảm đã mã hoá (KMS) nếu cần, Security Hub scan findings không còn critical.
* **Tối ưu chi phí:** Chi phí Genzite trong tầm kiểm soát, resource dư thừa đã được dọn dẹp.
* **Workshop Documentation:** Đạt 70% hoàn chỉnh sau Thứ 5 (VI+EN), demo screenshots đầy đủ các bước chính; hoàn thiện lên 90% vào Thứ 6.
* **Tổng kết:** Self-evaluation draft xong. **Genzite Project tổng tiến độ ~95% hoàn thành**. Hoàn thành Worklog Tuần 11.