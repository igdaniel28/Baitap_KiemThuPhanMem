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

---

## TC_AUTH_006 – Đăng nhập với mật khẩu sai

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_006 |
| **Tiêu đề** | Đăng nhập với mật khẩu sai |
| **Precondition** | Tài khoản đã tồn tại trong hệ thống |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu sai <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống thông báo đăng nhập thất bại |
| **Priority** | High |
| **Type** | Negative |

---

## TC_AUTH_007 – Đăng nhập với email không tồn tại

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_007 |
| **Tiêu đề** | Đăng nhập với email không tồn tại |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email chưa tồn tại trong hệ thống <br> 3. Nhập mật khẩu bất kỳ <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống thông báo tài khoản không tồn tại |
| **Priority** | High |
| **Type** | Negative |

---

## TC_AUTH_008 – Mật khẩu ít hơn 8 ký tự

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_008 |
| **Tiêu đề** | Đăng nhập với mật khẩu < 8 ký tự |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu có 7 ký tự <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống hiển thị thông báo mật khẩu không hợp lệ |
| **Priority** | Medium |
| **Type** | Boundary |

---

## TC_AUTH_009 – Kiểm tra SQL Injection tại ô đăng nhập

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_009 |
| **Tiêu đề** | Kiểm tra SQL Injection tại ô email |
| **Precondition** | Người dùng đang ở trang Login |
| **Steps** | 1. Truy cập trang Login <br> 2. Nhập email: `' OR '1'='1` <br> 3. Nhập mật khẩu bất kỳ <br> 4. Nhấn nút Login |
| **Expected Result** | Hệ thống từ chối đăng nhập và không bị bypass |
| **Priority** | High |
| **Type** | Negative |

---

## TC_AUTH_010 – Quên mật khẩu với email hợp lệ

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_010 |
| **Tiêu đề** | Gửi email đặt lại mật khẩu thành công |
| **Precondition** | Email đã tồn tại trong hệ thống |
| **Steps** | 1. Truy cập trang Quên mật khẩu <br> 2. Nhập email hợp lệ <br> 3. Nhấn nút Gửi |
| **Expected Result** | Hệ thống gửi email đặt lại mật khẩu |
| **Priority** | High |
| **Type** | Positive |

---

## TC_AUTH_011 – Quên mật khẩu với email không tồn tại

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_011 |
| **Tiêu đề** | Quên mật khẩu với email không tồn tại |
| **Precondition** | Người dùng đang ở trang Quên mật khẩu |
| **Steps** | 1. Truy cập trang Quên mật khẩu <br> 2. Nhập email không tồn tại <br> 3. Nhấn nút Gửi |
| **Expected Result** | Hệ thống hiển thị thông báo email không tồn tại |
| **Priority** | Medium |
| **Type** | Negative |

---

## TC_AUTH_011 – Quên mật khẩu với email không tồn tại

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_011 |
| **Tiêu đề** | Quên mật khẩu với email không tồn tại |
| **Precondition** | Người dùng đang ở trang Quên mật khẩu |
| **Steps** | 1. Truy cập trang Quên mật khẩu <br> 2. Nhập email không tồn tại <br> 3. Nhấn nút Gửi |
| **Expected Result** | Hệ thống hiển thị thông báo email không tồn tại |
| **Priority** | Medium |
| **Type** | Negative |

---

## TC_AUTH_012 – Đăng ký tài khoản với email hợp lệ

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_012 |
| **Tiêu đề** | Đăng ký với email hợp lệ |
| **Precondition** | Người dùng đang ở trang Đăng ký |
| **Steps** | 1. Truy cập trang Đăng ký <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu ≥ 8 ký tự <br> 4. Nhấn Đăng ký |
| **Expected Result** | Tạo tài khoản thành công |
| **Priority** | High |
| **Type** | Positive |

---

## TC_AUTH_013 – Đăng ký với email sai định dạng

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_013 |
| **Tiêu đề** | Đăng ký với email sai định dạng |
| **Precondition** | Người dùng đang ở trang Đăng ký |
| **Steps** | 1. Truy cập trang Đăng ký <br> 2. Nhập email: abc@ <br> 3. Nhập mật khẩu hợp lệ <br> 4. Nhấn Đăng ký |
| **Expected Result** | Hệ thống hiển thị lỗi định dạng email |
| **Priority** | Medium |
| **Type** | Negative |

---

## TC_AUTH_014 – Đăng ký với mật khẩu đúng 8 ký tự

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_014 |
| **Tiêu đề** | Đăng ký với mật khẩu đúng 8 ký tự |
| **Precondition** | Người dùng đang ở trang Đăng ký |
| **Steps** | 1. Truy cập trang Đăng ký <br> 2. Nhập email hợp lệ <br> 3. Nhập mật khẩu đúng 8 ký tự <br> 4. Nhấn Đăng ký |
| **Expected Result** | Đăng ký thành công |
| **Priority** | Medium |
| **Type** | Boundary |

---

## TC_AUTH_015 – Đăng xuất khỏi hệ thống

| Trường | Nội dung |
|------|----------|
| **TC_ID** | TC_AUTH_015 |
| **Tiêu đề** | Đăng xuất khỏi hệ thống |
| **Precondition** | Người dùng đã đăng nhập |
| **Steps** | 1. Nhấn nút Logout |
| **Expected Result** | Người dùng được đăng xuất và quay về trang Login |
| **Priority** | Low |
| **Type** | Positive |

