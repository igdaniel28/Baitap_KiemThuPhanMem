# TEST PLAN

## 1. Introduction

### 1.1 Mục đích tài liệu

Tài liệu Test Plan này được xây dựng nhằm mô tả kế hoạch kiểm thử thủ công (Manual Testing) cho **bài tập Chương 5 – Manual Testing theo nhóm dự án**. Tài liệu đóng vai trò định hướng toàn bộ hoạt động kiểm thử, giúp nhóm QA thực hiện kiểm thử một cách có hệ thống, nhất quán và có thể đánh giá chất lượng hệ thống trước khi đưa ra quyết định phát hành.

### 1.2 Đối tượng kiểm thử

Đối tượng được kiểm thử là **Website bán hàng online (E-commerce) giả lập**, được sử dụng phục vụ mục đích học tập. Hệ thống cho phép người dùng thực hiện các chức năng từ đăng ký tài khoản, tìm kiếm sản phẩm, quản lý giỏ hàng cho đến đặt hàng và xem lịch sử đơn hàng.

### 1.3 Mục tiêu kiểm thử

Mục tiêu chính của hoạt động kiểm thử trong chương 5 bao gồm:

* Xác minh các chức năng chính của hệ thống hoạt động đúng theo yêu cầu (Requirements)
* Phát hiện và ghi nhận các lỗi (bug) có thể ảnh hưởng đến trải nghiệm người dùng
* Đánh giá mức độ sẵn sàng của hệ thống trước khi phát hành (Release decision)
* Thực hành đầy đủ quy trình kiểm thử thủ công: Test Plan → Test Case → RTM → Bug Report → Test Report → Test Metrics

Tài liệu này là nền tảng để xây dựng các artefact kiểm thử khác trong chương 5 và được sử dụng xuyên suốt trong toàn bộ bài tập nhóm.

2. Scope
2.1 In-scope

Phạm vi kiểm thử của chương 5 bao gồm các chức năng chính của hệ thống Website bán hàng online (E-commerce), tập trung vào kiểm thử chức năng (Functional Testing), cụ thể:

Module Authentication

Đăng ký tài khoản

Đăng nhập

Quên mật khẩu

Đăng xuất

Module Product & Cart

Tìm kiếm sản phẩm

Lọc sản phẩm theo giá và danh mục

Xem chi tiết sản phẩm

Thêm sản phẩm vào giỏ hàng

Cập nhật số lượng sản phẩm trong giỏ

Xoá sản phẩm khỏi giỏ hàng

Module Checkout

Nhập địa chỉ giao hàng

Chọn phương thức thanh toán (COD / Visa giả lập)

Đặt hàng

Xem lịch sử đơn hàng

Ngoài ra, các kiểm tra giao diện cơ bản (UI basic) và kiểm tra hồi quy mức độ nhẹ (Smoke/Regression) cũng nằm trong phạm vi kiểm thử.

2.2 Out-of-scope

Các nội dung không thuộc phạm vi kiểm thử của bài tập này bao gồm:

Kiểm thử hiệu năng (Performance Testing)

Kiểm thử bảo mật chuyên sâu (Security / Penetration Testing)

Kiểm thử tự động (Automation Testing)

Kiểm thử khả năng chịu tải (Load / Stress Testing)

Tích hợp với các hệ thống thanh toán thật bên thứ ba

## 3. Test Approach

Dự án áp dụng phương pháp kiểm thử thủ công (Manual Testing) cho hệ thống website bán hàng online.

Các loại kiểm thử được thực hiện bao gồm:

- **Functional Testing**:  
  Kiểm tra các chức năng chính của hệ thống như đăng ký, đăng nhập, tìm kiếm sản phẩm, thêm giỏ hàng, thanh toán.

- **UI Testing (Basic)**:  
  Kiểm tra giao diện cơ bản, đảm bảo các nút, form, thông báo hiển thị đúng và dễ sử dụng.

- **Regression Testing (Smoke Test)**:  
  Kiểm tra nhanh các chức năng chính sau khi có thay đổi để đảm bảo hệ thống vẫn hoạt động ổn định.

## 4. Test Environment

- **Trình duyệt**: Google Chrome  
- **Hệ điều hành**: Windows  
- **Thiết bị**: Laptop / PC  
- **Dữ liệu kiểm thử**:  
  - Tài khoản người dùng giả lập  
  - Sản phẩm giả lập  
  - Thông tin thanh toán giả (COD / Visa giả lập)

## 5. Entry / Exit Criteria

### Entry Criteria
- Tài liệu yêu cầu đã sẵn sàng
- Môi trường kiểm thử được thiết lập
- Có dữ liệu test cần thiết

### Exit Criteria
- Tất cả test case quan trọng đã được thực thi
- Không còn lỗi mức độ Critical
- Báo cáo kiểm thử đã được hoàn thành

## 6. Risks & Mitigation

| Rủi ro | Mức độ | Biện pháp giảm thiểu |
|------|-------|----------------------|
| Yêu cầu thay đổi trong quá trình kiểm thử | Medium | Cập nhật test case và RTM kịp thời |
| Thiếu dữ liệu kiểm thử | Low | Giả lập dữ liệu test |
| Thời gian kiểm thử hạn chế | High | Ưu tiên test case quan trọng |

## 7. Roles & Responsibilities

| Vai trò | Trách nhiệm |
|------|-------------|
| Tester | Thiết kế và thực thi test case, báo cáo lỗi |
| Test Lead | Lập kế hoạch kiểm thử, tổng hợp báo cáo |
| Developer | Fix lỗi được báo cáo |

## 8. Test Schedule

| Giai đoạn | Thời gian |
|--------|-----------|
| Lập Test Plan | 1 ngày |
| Viết Test Case | 3 ngày |
| Thực thi kiểm thử | 3 ngày |
| Báo cáo & tổng kết | 1 ngày |

