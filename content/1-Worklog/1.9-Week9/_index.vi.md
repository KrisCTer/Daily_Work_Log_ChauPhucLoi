---
title: "Worklog Tuần 9"
date: 2026-06-19
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---



### Mục tiêu tuần 9:

* Hoàn thiện toàn bộ backend microservices (data-service, site-service, media-service, notification-service) và đạt 100% unit test coverage.
* Ổn định môi trường phát triển (dev runner, Kafka consumers, migrations sạch).
* Khởi động kiến trúc E-commerce (SaaS Billing, PayOS) và pipeline AI Generation thực tế qua Stitch SDK.

### Các công việc đã hoàn thành trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | **Data & Site Service:** <br> - Hoàn thiện data-service và Kafka events <br> - Triển khai backend canvas builder cho site-service <br> - Bổ sung AI agents, tích hợp MCP, BullMQ workers và tinh chỉnh pipeline ai-service | 15/06/2026 | 15/06/2026 |  |
| 3 | **Hoàn thiện Backend & Testing:** <br> - Triển khai media upload và notification services <br> - Ổn định build toàn dự án, xử lý shared-ui type generation, cô lập Prisma Client cho các service và sửa lỗi cú pháp trong gemini.client.ts <br> - Hoàn thiện toàn bộ 6 microservices và Gateway, triển khai JWT validation thật và đạt 100% unit test coverage | 16/06/2026 | 16/06/2026 |  |
| 4 | **Ổn định môi trường Dev:** <br> - Reset Prisma migrations về trạng thái sạch cho 6 service <br> - Thêm script concurrently để chạy đồng thời các service <br> - Sửa cấu hình Kafka consumer group và cập nhật docker-compose | 17/06/2026 | 17/06/2026 |  |
| 5 | **E-commerce Architecture:** <br> - Thêm commerce-service tích hợp PayOS <br> - Refactor App.tsx theo kiến trúc React mở rộng được <br> - Nâng cấp AI generation với Groq + RAG và triển khai SaaS Billing cùng Webhook Security cho identity-service | 18/06/2026 | 18/06/2026 |  |
| 6 | **AI Generate UI & Stitch SDK:** <br> - Cập nhật UI trang AI Generate qua nhiều vòng chỉnh sửa <br> - Tích hợp Stitch SDK (Google) và Groq Llama 3 cho việc sinh trang web tự động <br> - Thêm endpoint polling job, hỗ trợ preview HTML/ảnh trên Canvas và tích hợp MCP Tool Registry cho các AI client | 19/06/2026 | 19/06/2026 |  |

### Kết quả đạt được tuần 9:

* **Backend hoàn chỉnh:** Toàn bộ 6 microservices (identity, notification, site, data, media, ai) và Gateway đã hoàn thiện, đạt 100% unit test coverage và triển khai JWT validation thật.
* **Môi trường phát triển ổn định:** Dev runner có thể chạy đồng thời tất cả service, Kafka consumers hoạt động đúng và migrations Prisma ở trạng thái sạch trên toàn bộ hệ thống.
* **Kiến trúc E-commerce:** Khởi động commerce-service tích hợp cổng thanh toán PayOS và triển khai SaaS Billing kèm bảo mật Webhook.
* **AI Generation Pipeline:** Tích hợp thành công Stitch SDK + Groq Llama 3 cho việc sinh trang web tự động, hỗ trợ preview trực tiếp trên Canvas và chuẩn hóa MCP Tool Registry theo Genzite Design System.