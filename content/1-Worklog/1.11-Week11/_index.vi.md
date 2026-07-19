---
title: "Worklog Tuần 11"
date: 2026-07-03
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---



### Mục tiêu tuần 11:

* Hoàn thiện UI admin và Canvas Builder với metric generation thực, lưu lịch sử action vào DB.
* Tích hợp đăng nhập Cognito và upload ảnh qua Media service (S3), chuẩn hoá kiến trúc UI theo tiếng Anh.
* Gỡ bỏ commerce-service không cần thiết, thiết lập CI/CD production và áp dụng TypeScript strict toàn monorepo.

### Các công việc đã hoàn thành trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | **Admin UI:** <br> - Chỉnh sửa UI trang admin-identity-profile-notification | 29/06/2026 | 29/06/2026 |  |
| 3 | **Canvas & Builder hoàn thiện:** <br> - Tiếp tục refactor Canvas: lưu metric generation thực tế, lịch sử action động, loại bỏ mock data, lưu prompt vào DB <br> - Cập nhật UI Canvas Builder và cải thiện layout Login/Home/Dashboard <br> - Resolve conflict trong EditViewer.tsx và enforce English UI modular architecture | 30/06/2026 | 30/06/2026 |  |
| 4 | **Tích hợp Cognito & S3:** <br> - Hoàn thiện đăng nhập qua Cognito, upload ảnh từ Media service, chỉnh sửa ảnh đại diện profile và sửa lỗi đăng nhập | 01/07/2026 | 01/07/2026 |  |
| 5 | **Hoàn thiện Cognito & Chuẩn hoá i18n:** <br> - Resolve conflict EditViewer.tsx, triển khai UI cải thiện prompt, component-driven generation, cập nhật CanvasWorkspace và View Details metrics thời gian thực, quét regex đệ quy lấy URL ảnh lồng nhau trong widget <br> - Dịch toàn bộ string tiếng Việt hardcode sang tiếng Anh và dọn dead AI files <br> - Hoàn thiện tích hợp Cognito + S3, fix mặc định role VIEWER khi đăng ký qua SSO, chỉnh giao diện phần được giao và sửa lỗi thông báo/đổi mật khẩu | 02/07/2026 | 02/07/2026 |  |
| 6 | **Dọn dẹp & CI/CD Production:** <br> - Gỡ bỏ commerce-service không còn dùng, dọn dead code liên quan cả frontend/backend, cập nhật tài liệu kiến trúc theo mô hình 6-service <br> - Tạo Dockerfile production tối ưu cho pnpm workspaces và triển khai GitHub Actions deploy EC2 (backend) và S3 (frontend) <br> - Bật TypeScript strict (`noImplicitAny` và các rule strict khác), tạo interface chung `RequestWithUser`/`AuthUser`, fix lỗi kiểu ẩn trong `ai.consumer.ts` và `site-generator.service.ts` | 03/07/2026 | 03/07/2026 |  |

### Kết quả đạt được tuần 11:

* **Canvas Builder hoàn thiện:** Metric generation thời gian thực được lưu đúng, lịch sử action động thay thế toàn bộ mock data, prompt được lưu vào DB để truy vết.
* **Xác thực Cognito & Media:** Đăng nhập qua Amazon Cognito hoạt động ổn định, upload/chỉnh sửa ảnh đại diện qua Media service (S3) thành công, phân quyền mặc định VIEWER khi đăng ký qua SSO.
* **Chuẩn hoá codebase:** Toàn bộ chuỗi tiếng Việt hardcode được dịch sang tiếng Anh, kiến trúc UI module hoá theo chuẩn tiếng Anh.
* **Tối giản kiến trúc:** Gỡ bỏ hoàn toàn commerce-service không còn phù hợp, cập nhật tài liệu kiến trúc theo đúng mô hình 6-service.
* **CI/CD & Chất lượng code:** Thiết lập thành công CI/CD tự động (GitHub Actions deploy EC2 cho backend, S3 cho frontend), toàn bộ codebase đạt chuẩn TypeScript strict (`noImplicitAny`), tạo Dockerfile production tối ưu cho pnpm workspaces.