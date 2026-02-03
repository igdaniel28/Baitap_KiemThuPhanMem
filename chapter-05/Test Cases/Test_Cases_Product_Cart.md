# Test Cases – Product & Cart Module

Hệ thống: Website bán hàng online (E-commerce)  
Module: Product & Cart  

---

## TC_CART_001 – Tìm kiếm sản phẩm với từ khoá hợp lệ

| Trường | Nội dung |
|------|----------|
| TC_ID | TC_CART_001 |
| Tiêu đề | Tìm kiếm sản phẩm với từ khoá hợp lệ |
| Precondition | Có sản phẩm tồn tại trong hệ thống |
| Steps | 1. Nhập từ khoá hợp lệ vào ô tìm kiếm <br> 2. Nhấn Search |
| Expected Result | Danh sách sản phẩm phù hợp được hiển thị |
| Priority | High |
| Type | Positive |

---

## TC_CART_002 – Tìm kiếm với từ khoá không tồn tại

| Trường | Nội dung |
| TC_ID | TC_CART_002 |
| Tiêu đề | Tìm kiếm sản phẩm không tồn tại |
| Expected Result | Hiển thị thông báo không tìm thấy sản phẩm |
| Priority | Medium |
| Type | Negative |

---

## TC_CART_003 – Tìm kiếm với ký tự đặc biệt

| Trường | Nội dung |
| TC_ID | TC_CART_003 |
| Tiêu đề | Tìm kiếm với ký tự đặc biệt |
| Expected Result | Hệ thống không crash, xử lý an toàn |
| Priority | Medium |
| Type | Negative |

---

## TC_CART_004 – Lọc sản phẩm theo giá hợp lệ

| Trường | Nội dung |
| TC_ID | TC_CART_004 |
| Tiêu đề | Lọc theo khoảng giá hợp lệ |
| Expected Result | Chỉ hiển thị sản phẩm trong khoảng giá |
| Priority | High |
| Type | Positive |

---

## TC_CART_005 – Lọc theo giá min > max

| Trường | Nội dung |
| TC_ID | TC_CART_005 |
| Tiêu đề | Lọc theo giá không hợp lệ |
| Expected Result | Hiển thị thông báo lỗi |
| Priority | Medium |
| Type | Boundary |

---

## TC_CART_006 – Lọc theo danh mục

| Trường | Nội dung |
| TC_ID | TC_CART_006 |
| Tiêu đề | Lọc sản phẩm theo danh mục |
| Expected Result | Hiển thị đúng sản phẩm theo danh mục |
| Priority | High |
| Type | Positive |

---

## TC_CART_007 – Xem chi tiết sản phẩm

| Trường | Nội dung |
| TC_ID | TC_CART_007 |
| Tiêu đề | Xem chi tiết sản phẩm |
| Expected Result | Hiển thị đầy đủ thông tin sản phẩm |
| Priority | High |
| Type | Positive |

---

## TC_CART_008 – Xem chi tiết sản phẩm không tồn tại

| Trường | Nội dung |
| TC_ID | TC_CART_008 |
| Tiêu đề | Xem sản phẩm không tồn tại |
| Expected Result | Hiển thị trang lỗi hoặc thông báo phù hợp |
| Priority | Medium |
| Type | Negative |

---

## TC_CART_009 – Thêm sản phẩm vào giỏ hàng

| Trường | Nội dung |
| TC_ID | TC_CART_009 |
| Tiêu đề | Thêm sản phẩm vào giỏ |
| Expected Result | Sản phẩm được thêm vào giỏ thành công |
| Priority | High |
| Type | Positive |

---

## TC_CART_010 – Thêm sản phẩm trùng vào giỏ

| Trường | Nội dung |
| TC_ID | TC_CART_010 |
| Tiêu đề | Thêm sản phẩm đã có trong giỏ |
| Expected Result | Tăng số lượng sản phẩm |
| Priority | Medium |
| Type | Boundary |

---

## TC_CART_011 – Cập nhật số lượng hợp lệ

| Trường | Nội dung |
| TC_ID | TC_CART_011 |
| Tiêu đề | Cập nhật số lượng sản phẩm |
| Expected Result | Số lượng được cập nhật đúng |
| Priority | High |
| Type | Positive |

---

## TC_CART_012 – Cập nhật số lượng = 0

| Trường | Nội dung |
| TC_ID | TC_CART_012 |
| Tiêu đề | Cập nhật số lượng bằng 0 |
| Expected Result | Sản phẩm bị xoá khỏi giỏ |
| Priority | Medium |
| Type | Boundary |

---

## TC_CART_013 – Cập nhật số lượng âm

| Trường | Nội dung |
| TC_ID | TC_CART_013 |
| Tiêu đề | Cập nhật số lượng âm |
| Expected Result | Hiển thị lỗi validation |
| Priority | Medium |
| Type | Negative |

---

## TC_CART_014 – Xoá sản phẩm khỏi giỏ hàng

| Trường | Nội dung |
| TC_ID | TC_CART_014 |
| Tiêu đề | Xoá sản phẩm khỏi giỏ |
| Expected Result | Sản phẩm bị xoá thành công |
| Priority | High |
| Type | Positive |

---

## TC_CART_015 – Giỏ hàng rỗng

| Trường | Nội dung |
| TC_ID | TC_CART_015 |
| Tiêu đề | Hiển thị giỏ hàng rỗng |
| Expected Result | Hiển thị thông báo giỏ hàng trống |
| Priority | Low |
| Type | Positive |

---

## TC_CART_016 – Tổng tiền giỏ hàng chính xác

| Trường | Nội dung |
| TC_ID | TC_CART_016 |
| Tiêu đề | Tính tổng tiền giỏ hàng |
| Expected Result | Tổng tiền hiển thị chính xác |
| Priority | High |
| Type | Positive |

---

## TC_CART_017 – Tổng tiền cập nhật khi thay đổi số lượng

| Trường | Nội dung |
| TC_ID | TC_CART_017 |
| Tiêu đề | Cập nhật tổng tiền |
| Expected Result | Tổng tiền thay đổi đúng |
| Priority | High |
| Type | Boundary |

---

## TC_CART_018 – Thêm sản phẩm khi chưa đăng nhập

| Trường | Nội dung |
| TC_ID | TC_CART_018 |
| Tiêu đề | Thêm sản phẩm khi chưa đăng nhập |
| Expected Result | Yêu cầu đăng nhập |
| Priority | High |
| Type | Negative |

---

## TC_CART_019 – Giữ giỏ hàng sau khi reload trang

| Trường | Nội dung |
| TC_ID | TC_CART_019 |
| Tiêu đề | Lưu trạng thái giỏ hàng |
| Expected Result | Giỏ hàng được giữ nguyên |
| Priority | Medium |
| Type | Positive |

---

## TC_CART_020 – Xoá toàn bộ giỏ hàng

| Trường | Nội dung |
| TC_ID | TC_CART_020 |
| Tiêu đề | Xoá toàn bộ sản phẩm trong giỏ |
| Expected Result | Giỏ hàng trống |
| Priority | Medium |
| Type | Positive |
