# Mô hình quan hệ dữ liệu
## 1. Overview
- **Mô hình dữ liệu** là tập các dữ liệu được mô tả gồm 3 phần:
  1. Cấu trúc của dữ liệu
  2. Toán tử của dữ liệu
  3. Liên hệ ràng buộc của dữ liệu.
- **Mô hình quan hệ** gồm 2 phần:
  1. Lược đồ
  2. Trường hợp.

![image](<Pictures_Source/Picture6.png>)

- **Cách biểu diễn DB Scheme**:

![image](<Pictures_Source/Picture7.png>)

## 2. Cấu trúc quan hệ cơ bản
**Đại số quan hệ**
1. $$R\cup S = \{t|t\in R\lor t\in S\}$$
2. $$R\cap S = \{t|t\in R\land t\in S\}$$
3. $$R\\S = \{t|t\in R\land t\notin S\}$$
4. $$R\times S$$
5. $$R\div V$$
6. Selection: xử lý có điều kiện. $$R1 = \sigma_{condition}(R2)$$
7. Projection: sử dụng để lấy cột $$S = \pi_{A_1,A_2,...,A_n}(R)$$
8. $$\theta$$ joins: Tích Decarse có điều kiện $$R_3 = R1\space ⋈_{\<join condition\>} R_2$$
9. Natural join: Tích tự nhiên, 2 cột nào có giá trị bằng nhau thì lấy, bỏ cột trùng lặp $$R_3 = R1\space ⋈\space R_2$$
10. Rename: $$P$$

## Excercise

a) $$\pi_{model,speed}(\sigma_{speed\ge 3.00}(PC))$$

(*)b) $$\pi_{model,ram,hd,screen}(\sigma_{hd\ge 100}(Laptop))$$

(*)c) $$\pi_{}$$
