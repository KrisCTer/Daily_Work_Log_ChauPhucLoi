---
title: "Worklog Tuần 12"
date: 2026-07-10
weight: 12
chapter: false
pre: " <b> 1.12 </b> "
---


### Mục tiêu tuần 12:

* Triển khai production hoàn chỉnh: Nginx reverse proxy, sửa toàn bộ lỗi deploy Docker/Prisma, cấu hình biến môi trường.
* Vá các lỗi vận hành phát sinh sau deploy (API response format, quyền truy cập, upload media, đường link public).
* Hoàn thiện Genzite Project 100%, nộp báo cáo tốt nghiệp FCJ đầy đủ 7 mục.
* Dùng các ngày tiếp theo làm thời gian bù nếu deploy hoặc testing chậm tiến độ.

### Các công việc đã hoàn thành trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                         |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ---------------------------------------------------------------------- |
| 2   | **Thiết lập triển khai Production:** <br> - Thiết lập Nginx reverse proxy, sửa routing API frontend, fix Dockerfile thiếu thư mục dist, loại bỏ volume mount local ở production <br> - Sửa lỗi Prisma generate/migrate deploy (thêm flag `--yes`, bypass npx, cài Prisma CLI global, pin Prisma CLI về v6 để tương thích schema) <br> - Fix Nginx DNS cache bằng Docker resolver, bổ sung biến môi trường còn thiếu (`ms`, `KAFKA_CONSUMER_GROUP`, `EMAIL_USERNAME`, `EMAIL_PASSWORD`) và cấu hình Nginx với security headers + gzip cho frontend/API | 06/07/2026   | 06/07/2026      | [github.com/KrisCTer/Genzite](https://github.com/KrisCTer/Genzite.git) |
| 3   | **Sửa lỗi vận hành & kiểm thử:** <br> - Test regression toàn bộ chức năng chính trên môi trường production (đăng ký/đăng nhập, tạo trang AI, chỉnh sửa CMS, publish, upload media) <br> - Vá các lỗi crash do response API không đồng nhất, xử lý vấn đề access control cho 403 overlay và quyền collaborator/viewer, đồng thời sửa lỗi upload media qua presigned URL <br> - Rà soát và đóng các issue còn tồn đọng sau đợt deploy lớn và dọn dẹp tài nguyên thử nghiệm không cần dùng                                                               | 07/07/2026   | 07/07/2026      | [github.com/KrisCTer/Genzite](https://github.com/KrisCTer/Genzite.git) |
| 4   | **Tinh chỉnh Canvas & live viewer:** <br> - Thêm component `CanvasPageFrame` (undo/redo, responsive viewport), triển khai `EditViewer` tích hợp GrapesJS và cải thiện trải nghiệm live viewer <br> - Hoàn thiện `ThemeEditorPanel`, design system generator, animation lưu GrapesJS, cảnh báo unsaved changes và làm publish domains dynamic theo hostname <br> - Sửa nhiều lỗi TypeScript/React Hook, dùng biến môi trường cho invite email link và cải thiện redirect login trên public subdomain                                                   | 08/07/2026   | 08/07/2026      | [workshop-sample.fcjuni.com](https://workshop-sample.fcjuni.com)       |
| 5   | **Chuẩn bị tài liệu & báo cáo cuối khóa:** <br> - Hoàn thiện Workshop Documentation 100% (song ngữ VI/EN), chốt sơ đồ kiến trúc cuối cùng của hệ thống 6-service <br> - Hoàn thiện Proposal Genzite Project 100%, viết đầy đủ Self-evaluation 8 tiêu chí FCJ và biên soạn báo cáo FCJ 7 mục <br> - Review lần cuối toàn bộ tài liệu trước khi nộp                                                                                                                                                                                                     | 09/07/2026   | 09/07/2026      | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)       |
| 6   | **Nộp báo cáo cuối khóa / ngày bù:** <br> - Submit báo cáo FCJ đầy đủ 7 mục lên hệ thống <br> - Dùng các ngày tiếp theo làm thời gian bù nếu deploy hoặc testing cần thêm kiểm tra                                                                                                                                                                                                                                                                                                                                                                    | 10/07/2026   | 12/07/2026      | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)       |

### Kết quả đạt được tuần 12:

* **Production ổn định:** Toàn bộ hệ thống Genzite chạy ổn định trên môi trường production qua Nginx reverse proxy, loạt lỗi deploy Docker/Prisma đã được xử lý triệt để.
* **Vận hành mượt mà:** Các lỗi phát sinh sau deploy (crash do response API, quyền truy cập, upload media qua S3) đã được vá kịp thời, hệ thống hoạt động ổn định cho người dùng thật.
* **Genzite Project DONE 100%:** Test regression toàn diện, không còn lỗi nghiêm trọng, demo trơn tru.
* **Tài liệu hoàn chỉnh:** Workshop Documentation 100% (VI+EN), Proposal 100%, Self-evaluation đầy đủ 8 tiêu chí.
* **Nộp báo cáo thành công:** Báo cáo FCJ đầy đủ 7 mục nộp đúng hạn, LinkedIn cập nhật, chia sẻ hành trình 12 tuần. **HOÀN THÀNH CHƯƠNG TRÌNH**