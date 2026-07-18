---
title: "Worklog Tuần 6"
date: 2026-05-29
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---



### Mục tiêu tuần 6:

* Đào sâu kiến thức Cơ sở dữ liệu trên AWS: RDS engines, Multi-AZ (High Availability), Read Replica (performance), và Aurora Serverless v2.
* Thực hành Database Migration Service (DMS): Schema Conversion Tool, migration Full Load + CDC.
* Triển khai PROJECT 1 (Personal Blog Website) kết hợp EC2, RDS, S3 và IAM Role từ hạ tầng các tuần trước.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                      |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------------------------------------------------- |
| 2   | **VIDEO FCJ BOOTCAMP:** <br> - Module 06-01: Database Concepts review – relational vs NoSQL, ACID <br> - Module 06-02: Amazon RDS & Aurora – engines, Multi-AZ, Read Replica <br> **THỰC HÀNH & HỌC THÊM:** <br> - Tìm hiểu Amazon RDS: engines (MySQL/PostgreSQL), Multi-AZ, Read Replica <br> - Lab: tạo RDS MySQL db.t3.micro trong private subnet <br> - Kết nối RDS từ EC2 bằng MySQL client <br> **LAB & GHI CHÚ:** <br> - Ghi chú: RDS engines (MySQL/PG/Oracle/MSSQL/Aurora), backup retention                  | 25/05/2026   | 25/05/2026      | |
| 3   | **VIDEO FCJ BOOTCAMP:** <br> - Module 06-03: Redshift - ElastiCache <br> - Lab05-2.1→7: RDS thực hành – VPC, SG, Subnet Group, EC2, RDS, App Deploy, Backup, Cleanup <br> **THỰC HÀNH & HỌC THÊM:** <br> - Tìm hiểu RDS Multi-AZ (High Availability) và Read Replica (performance) <br> - Test failover Multi-AZ, đo độ trễ Read Replica <br> - Backup/restore, automated snapshot <br> **LAB & GHI CHÚ:** <br> - Lab 000005: Amazon Relational Database Service (Amazon RDS)                                              | 26/05/2026   | 26/05/2026      | [000005.awsstudygroup.com](https://000005.awsstudygroup.com/) |
| 4   | **VIDEO FCJ BOOTCAMP:** <br> - Lab43-01→17: Database Migration Service (DMS) – RDP, Fleet Manager, MSSQL/Oracle config, Schema Conversion, Migration Task, Troubleshoot <br> **THỰC HÀNH & HỌC THÊM:** <br> - Tìm hiểu Database Migration Service (DMS): Homogeneous vs Heterogeneous migration <br> - Sử dụng Schema Conversion Tool (SCT) <br> - Tạo migration task Full Load + CDC <br> **LAB & GHI CHÚ:** <br> - Lab 000043: Database Schema Conversion & Migration <br> - Ghi chú: Homogeneous vs Heterogeneous migration, SCT tool | 27/05/2026   | 27/05/2026      | [000043.awsstudygroup.com](https://000043.awsstudygroup.com/) |
| 5   | **THỰC HÀNH & HỌC THÊM:** <br> - **PROJECT 1: Personal Blog Website (bắt đầu)** <br> - Deploy EC2 (t2.micro) trong VPC đã tạo (Module 2) <br> - Cài WordPress/Nginx + kết nối RDS MySQL (Module 6) <br> - Lưu media lên S3 (Module 4), phân quyền IAM Role cho EC2 (Module 5) <br> - Cấu hình Security Group đúng principle <br> **LAB & GHI CHÚ:** <br> - Deploy EC2 trong VPC tuần 2, cài WordPress/Nginx <br> - IAM Role cho EC2 truy cập S3 (media bucket)                                                                                      | 28/05/2026   | 28/05/2026      | [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/)           |
| 6   | **THỰC HÀNH & HỌC THÊM:** <br> - Hoàn thiện PROJECT 1: Personal Blog (EC2+RDS+S3+IAM Role), ước tính cost ~$25/tháng <br> - Viết tài liệu Project 1: kiến trúc, chi phí <br> - Viết Worklog Tuần 6 – tổng hợp Module 6 (Database) <br> - Cleanup RDS test không cần dùng tiếp <br> **LAB & GHI CHÚ:** <br> - PROJECT 1: Personal Blog (EC2 + RDS + S3 + IAM Role) <br> - Viết Worklog Tuần 6                                                                                                                                                        | 29/05/2026   | 29/05/2026      | [rules.fcjuni.com/3-project](https://rules.fcjuni.com/3-project)                    |


### Kết quả đạt được tuần 6:
* **Nền tảng Database:** Phân biệt rõ Multi-AZ (HA) vs Read Replica (performance), hiểu cơ chế Aurora Serverless v2, RDS instance đang AVAILABLE, kết nối thành công từ EC2, CRUD query hoạt động.
* **Thực hành RDS:** RDS MySQL db.t3.micro chạy trong private subnet, app kết nối RDS từ EC2 thành công, snapshot restore test OK, test failover Multi-AZ thành công. Hoàn thành Lab 000005.
* **Database Migration Service:** MSSQL → Aurora MySQL migration thành công, Schema Conversion Tool chạy được, hiểu rõ Full Load vs CDC migration mode. Hoàn thành Lab 000043.
* **PROJECT 1 (Personal Blog):** Blog website truy cập được qua IP, S3 lưu media, RDS lưu data, IAM Role áp dụng đúng (không dùng Access Key), có ảnh chụp màn hình demo đầy đủ.
* **Tổng kết:** PROJECT 1 hoàn thành, demo được, tài liệu Project 1 hoàn chỉnh. Module 6 hoàn thành 2/2 lab. Hoàn thành Worklog Tuần 6.