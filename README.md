# Bộ Mô Phỏng Trực Quan Thuật Toán & Cấu Trúc Dữ Liệu
> **Môn học:** Cấu trúc dữ liệu & Giải thuật  
> **Khoa Công nghệ Thông tin - Trường ĐH Sư Phạm TP.HCM (HCMUE)**  
> **Ứng dụng:** Mô phỏng từng pass/bước (Step-by-step Execution Engine)

---

## 📂 Danh mục tài nguyên
- `index.html`: Ứng dụng web trực quan standalone, chạy offline 100% trên trình duyệt (Chrome, Edge, Firefox, Cốc Cốc,...).
- `../mo_phong_ctdl.html`: Bản sao ứng dụng tại thư mục gốc `homework` để mở nhanh.

---

## 🎯 Phân bổ Nội dung & Chuẩn Đầu Ra (CLO 1 - CLO 5)

| Phần | Nội dung học phần | Thuật toán / Thao tác mô phỏng | Chuẩn đầu ra (CLO) |
|---|---|---|---|
| **Chương 1** | Giới thiệu ADT & Độ phức tạp | Bảng phân tích thời gian Best / Avg / Worst & Không gian Space | **CLO 2** (Vận dụng kiến thức cơ bản) |
| **Chương 2** | Tìm kiếm (Searching) | - Linear Search<br>- Binary Search (Left, Right, Mid) | **CLO 4** (Cài đặt giải thuật tìm kiếm) |
| **Chương 2** | Sắp xếp (Sorting) | - Bubble Sort (Cơ bản & Cải tiến `haveSwap`)<br>- Selection Sort (Chọn trực tiếp `min_idx`)<br>- Interchange Sort (Đổi chỗ trực tiếp)<br>- Insertion Sort (Chèn trực tiếp)<br>- Merge Sort (Chia để trị & Trộn)<br>- Heap Sort (Max-Heap & Vun đống `heapify`)<br>- Quick Sort (Phân hoạch `partition`)<br>- **Radix Sort** (Cơ số LSD: Giá đỡ 10 thùng chữ số 0-9) | **CLO 4** (Cài đặt giải thuật sắp xếp) |
| **Chương 3** | Danh sách liên kết (Linked Lists) | - Singly Linked List (Duyệt, In ngược đệ quy Call Stack)<br>- Sorted Insert (Chèn có thứ tự `newNode`)<br>- Delete Node (Xóa phần tử theo khóa)<br>- Doubly Linked List (DSLK Đôi 2 chiều `prev` & `next`) | **CLO 3, CLO 5** (Thao tác trên DSLK) |
| **Chương 4** | Ngăn xếp - Hàng đợi (Stack & Queue) | - Stack ADT (LIFO: Push, Pop, Peek)<br>- **RPN Calculator** (Tính biểu thức hậu tố từng token)<br>- Queue ADT (FIFO: Enqueue, Dequeue)<br>- Circular Queue | **CLO 3, CLO 5** (Thao tác trên Stack/Queue) |
| **Chương 5** | Cấu trúc Cây (Trees) | - Binary Search Tree (Chèn, Tìm kiếm, Tìm Min/Max)<br>- Tree Traversals: NLR (Pre), LNR (Inorder tăng dần), LRN (Post), BFS Level-Order (Queue)<br>- **AVL Tree**: Chiều cao $h$, Hệ số cân bằng $BF = h_L - h_R$, 4 phép quay LL, RR, LR, RL | **CLO 3, CLO 5** (Thao tác trên Cây BST & AVL) |
| **Chương 6** | Bảng băm (Hash Table) | - Hàm băm $h(k) = k \pmod M$<br>- Xử lý đụng độ bằng Chaining (DSLK)<br>- Xử lý đụng độ bằng Linear Probing (Địa chỉ mở) | **CLO 3, CLO 5** (Thao tác trên Bảng băm) |
| **Tổng kết** | Bài tập lớn & Đồ án nhóm | Ma trận phân công nhiệm vụ, cấu trúc dự án & báo cáo chuẩn | **CLO 1** (Làm việc nhóm & BTL) |

---

## 🚀 Hướng Dẫn Sử Dụng
1. Nhấp đúp chuột mở file `index.html` (hoặc `mo_phong_ctdl.html`).
2. Chọn tab nội dung mong muốn (Tìm kiếm, Sắp xếp, DSLK, Stack/Queue, Cây, Bảng băm, Chuẩn đầu ra).
3. Sử dụng các nút điều khiển:
   - `|<<`: Về bước đầu tiên.
   - `<`: Lùi 1 bước logic.
   - `▶ Tự chạy`: Tự động chạy theo tốc độ điều chỉnh.
   - `>`: Tiến 1 bước logic (Pass kế tiếp hoặc so sánh/hoán đổi kế tiếp).
   - `>>|`: Nhảy thẳng đến kết quả hoàn thành.
   - `🔄 Reset`: Đặt lại mảng/dữ liệu ban đầu.
4. Có thể nhập dữ liệu tùy ý (Mảng số, Giá trị tìm kiếm, Giá trị chèn/xóa) hoặc bấm `🎲 Ngẫu nhiên`.
5. Quan sát đồng thời:
   - **Giai đoạn trực quan**: Màu sắc thay đổi trực quan (Vàng: Đang so sánh; Đỏ: Hoán đổi; Xanh lá: Đã có thứ tự chuẩn; Tím: Pivot/Node mới).
   - **Thuyết minh từng pass**: Giải thích chi tiết bằng tiếng Việt.
   - **Bảng biến**: Theo dõi thời gian thực các biến `i`, `j`, `mid`, `min_idx`, `top`, `front`, `rear`, `BF`,...
   - **Mã nguồn C++**: Highlight dòng code đang chạy.
