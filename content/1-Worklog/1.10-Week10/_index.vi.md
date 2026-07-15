---
title: "Worklog Tuần 10"
date: 2026-06-26
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:

* Học nhẹ (chỉ tra cứu khi cần), tập trung hoàn thiện API/Frontend và tích hợp toàn bộ các layer của Genzite Project.
* Xây dựng hoàn chỉnh API layer cho CMS và AI generation, kết nối với Frontend React/TypeScript.
* Tích hợp Networking (VPC/Security Group) và test tích hợp toàn diện toàn bộ hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                             |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2   | **GENZITE:** <br> - Xây dựng/hoàn thiện API layer (REST API NestJS controllers) <br> - Định nghĩa đầy đủ endpoints cho CMS + AI generation (GET/POST/PUT/DELETE) <br> **TRA CỨU NHANH (khi cần):** <br> - API design best practices – 10-15 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000022.awsstudygroup.com                                      | 22/06/2026   | 22/06/2026      | [000022.awsstudygroup.com](https://000022.awsstudygroup.com/)                                                                                                              |
| 3   | **GENZITE:** <br> - Hoàn thiện Frontend (React/TypeScript) gọi API <br> - Kết nối Frontend ↔ API layer (CMS editor + AI generation UI) <br> **LAB & GHI CHÚ:** <br> - Tham khảo: cloudjourney.awsstudygroup.com                                                                                                                                          | 23/06/2026   | 23/06/2026      | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/)                                                                                                  |
| 4   | **GENZITE:** <br> - Tích hợp Networking (VPC/Security Group) đảm bảo bảo mật cho toàn hệ thống <br> - Review lại Security Group, IAM Role toàn bộ kiến trúc (ai-service, backend, database) <br> **HỌC NHẸ:** <br> - Ôn VPC Endpoint cho dịch vụ nội bộ – 20 phút <br> **LAB & GHI CHÚ:** <br> - Tham khảo: 000003.awsstudygroup.com                     | 24/06/2026   | 24/06/2026      | [000003.awsstudygroup.com](https://000003.awsstudygroup.com/)                                                                                                              |
| 5   | **GENZITE:** <br> - Test tích hợp toàn diện (integration test) toàn bộ hệ thống <br> - Test các use-case chính: tạo website AI, chỉnh sửa CMS, publish <br> - Ghi nhận và fix bug phát sinh <br> **LAB & GHI CHÚ:** <br> - Tham khảo: cloudjourney.awsstudygroup.com                                                                                     | 25/06/2026   | 25/06/2026      | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/)                                                                                                  |
| 6   | **THỰC HÀNH & HỌC THÊM:** <br> - Review toàn bộ tiến độ Genzite (Backend+Storage+API+Frontend) <br> - Viết Worklog Tuần 10 <br> - Cập nhật Proposal Genzite (gần hoàn chỉnh) <br> - Bắt đầu phác thảo Workshop Documentation (FCJ Hugo template) <br> **LAB & GHI CHÚ:** <br> - github.com/thienluhoan/fcj-workshop-template <br> - Viết Worklog Tuần 10 | 26/06/2026   | 26/06/2026      | [github.com/thienluhoan/fcj-workshop-template](https://github.com/thienluhoan/fcj-workshop-template) <br> [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project) |


### Kết quả đạt được tuần 10:

* **API Layer:** API endpoints đầy đủ chức năng chính, test bằng Postman/curl thành công.
* **Tích hợp Frontend:** Frontend hiển thị và gọi API thành công, UI cơ bản đầy đủ chức năng chính.
* **Networking & Bảo mật:** Toàn bộ traffic đi đúng qua subnet/SG quy định, không có lỗ hổng quyền truy cập rõ ràng.
* **Test tích hợp:** Hệ thống chạy ổn định end-to-end, các bug chính đã được fix.
* **Tổng kết:** Genzite Project ~75% hoàn chỉnh. Proposal Genzite 85%. Workshop doc draft 20%. Hoàn thành Worklog Tuần 10.