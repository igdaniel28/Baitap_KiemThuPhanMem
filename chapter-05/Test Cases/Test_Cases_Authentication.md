# Test Cases – Authentication Module

## Thông tin chung
- Module: Authentication
- Chức năng: Đăng ký, Đăng nhập, Quên mật khẩu, Đăng xuất
- Tổng số test case dự kiến: 15
---

## TC_AUTH_001 – Đăng nhập với thông tin hợp lệ

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_001 |
| **Tiêu đề** | Đăng nhập với thông tin hợp lệ |
| **Precondition** | Người dùng đã có tài khoản hợp lệ |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu đúng <br> 4. Nhấn nút Login |
| **Expected Result** | Người dùng đăng nhập thành công và được chuyển đến trang chủ |
| **Priority** | High |
| **Type** | Positive |

---

## TC_AUTH_002 – Đăng nhập với mật khẩu sai

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_002 |
| **Tiêu đề** | Đăng nhập với mật khẩu sai |
| **Precondition** | Người dùng đã có tài khoản hợp lệ |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu sai <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống hiển thị thông báo lỗi và không cho đăng nhập |
| **Priority** | High |
| **Type** | Negative |

---

## TC_AUTH_003 – Đăng nhập khi bỏ trống email

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_003 |
| **Tiêu đề** | Đăng nhập khi bỏ trống email |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Để trống trường email <br> 3. Nhập mật khẩu hợp lệ <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống hiển thị thông báo yêu cầu nhập email |
| **Priority** | Medium |
| **Type** | Negative |

---

## TC_AUTH_004 – Đăng nhập khi bỏ trống mật khẩu

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_004 |
| **Tiêu đề** | Đăng nhập khi bỏ trống mật khẩu |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email hợp lệ <br> 3. Để trống trường mật khẩu <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống hiển thị thông báo yêu cầu nhập mật khẩu |
| **Priority** | Medium |
| **Type** | Negative |

---

## TC_AUTH_005 – Đăng nhập với email sai định dạng

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_005 |
| **Tiêu đề** | Đăng nhập với email sai định dạng |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email sai định dạng (vd: abc@) <br> 3. Nhập mật khẩu hợp lệ <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống hiển thị thông báo email không hợp lệ |
| **Priority** | Medium |
| **Type** | Negative |


