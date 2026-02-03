# Test Cases – Checkout Module

Hệ thống: Website bán hàng online (E-commerce)  
Module: Checkout  

---

### TC_CHECKOUT_001
**Title:** Thanh toán thành công với đầy đủ thông tin hợp lệ  
**Precondition:** User đã đăng nhập, giỏ hàng có sản phẩm  
**Steps:**
1. Đi đến trang Checkout
2. Nhập địa chỉ giao hàng hợp lệ
3. Chọn phương thức COD
4. Nhấn Đặt hàng  
**Expected Result:** Đặt hàng thành công  
**Priority:** High  
**Type:** Positive  

---

### TC_CHECKOUT_002
**Title:** Không cho đặt hàng khi chưa nhập địa chỉ  
**Precondition:** User đã đăng nhập, giỏ hàng có sản phẩm  
**Steps:**
1. Đi đến Checkout
2. Bỏ trống địa chỉ
3. Nhấn Đặt hàng  
**Expected Result:** Hiển thị thông báo lỗi  
**Priority:** High  
**Type:** Negative  

---

### TC_CHECKOUT_003
**Title:** Chọn phương thức thanh toán COD  
**Precondition:** User ở trang Checkout  
**Steps:**
1. Chọn COD
2. Tiếp tục đặt hàng  
**Expected Result:** COD được chấp nhận  
**Priority:** Medium  
**Type:** Positive  

---

### TC_CHECKOUT_004
**Title:** Chọn thanh toán Visa giả lập  
**Precondition:** User ở trang Checkout  
**Steps:**
1. Chọn Visa
2. Nhập thông tin thẻ giả lập
3. Nhấn Continue  
**Expected Result:** Chuyển sang trang xác nhận  
**Priority:** Medium  
**Type:** Positive  

---

### TC_CHECKOUT_005
**Title:** Không cho tiếp tục khi thiếu thông tin thanh toán  
**Precondition:** Chọn Visa  
**Steps:**
1. Không nhập số thẻ
2. Nhấn Continue  
**Expected Result:** Báo lỗi validation  
**Priority:** High  
**Type:** Negative  

---

### TC_CHECKOUT_006
**Title:** Hiển thị đúng danh sách sản phẩm khi Checkout  
**Precondition:** Có nhiều sản phẩm trong giỏ  
**Steps:**
1. Đi đến Checkout  
**Expected Result:** Hiển thị đúng sản phẩm và số lượng  
**Priority:** Medium  
**Type:** Positive  

---

### TC_CHECKOUT_007
**Title:** Hiển thị đúng tổng tiền đơn hàng  
**Precondition:** Có nhiều sản phẩm trong giỏ  
**Steps:**
1. Mở trang Checkout  
**Expected Result:** Tổng tiền chính xác  
**Priority:** High  
**Type:** Boundary  

---

### TC_CHECKOUT_008
**Title:** Không cho đặt hàng khi giỏ hàng trống  
**Precondition:** Giỏ hàng trống  
**Steps:**
1. Truy cập Checkout  
**Expected Result:** Không thể tiếp tục  
**Priority:** High  
**Type:** Negative  

---

### TC_CHECKOUT_009
**Title:** Lưu đơn hàng sau khi đặt thành công  
**Precondition:** Đặt hàng thành công  
**Steps:**
1. Truy cập lịch sử đơn hàng  
**Expected Result:** Đơn hàng được lưu  
**Priority:** Medium  
**Type:** Positive  

---

### TC_CHECKOUT_010
**Title:** Hiển thị thông báo xác nhận đặt hàng  
**Precondition:** Đặt hàng thành công  
**Steps:**
1. Hoàn tất thanh toán  
**Expected Result:** Hiển thị thông báo thành công  
**Priority:** Low  
**Type:** Positive  
