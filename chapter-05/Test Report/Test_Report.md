# Test Report

## 1. Tổng quan
Hệ thống: Website bán hàng online (E-commerce)  
Phạm vi kiểm thử: Authentication, Product & Cart, Checkout  

---

## 2. Thống kê Test Case

| Tổng TC | Pass | Fail | Blocked |
|-------|------|------|---------|
| 45 | 35 | 10 | 0 |

Execution Rate = 100%

---

## 3. Top lỗi nghiêm trọng

1. BUG_CART_001 – Sai tổng tiền giỏ hàng (Critical)
2. BUG_CHECKOUT_001 – Không validate địa chỉ (Critical)
3. BUG_AUTH_001 – Email sai định dạng vẫn đăng ký
4. BUG_CART_003 – Cho phép số lượng âm
5. BUG_ORDER_001 – Không lưu lịch sử đơn hàng

---

## 4. Đánh giá chất lượng
Hệ thống còn tồn tại các lỗi nghiêm trọng ảnh hưởng trực tiếp đến chức năng đặt hàng và thanh toán.

---

## 5. Kết luận
❌ **No-Release**  
Hệ thống **chưa đủ điều kiện phát hành** do còn lỗi Critical.
