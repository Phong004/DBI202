# Mô hình database
- Xác định các Getting User Requirment: viết ra 1 cái bảng tổng quát, có các thành phần và liên hệ nào (Đặc tả)
- Thiết kế mức độ khái niệm. (Sơ đồ ERD)
## ERD 
1. Xác định các dữ liệu cần mô hình hóa
2. Xác định các dữ liệu có thể mô hình hóa trong thế giới thật
3. Xác định các thuộc tính của từng thực thể
4. Sắp xếp các tập thực thể là tập yếu hoặc tập mạnh
5. Sắp xếp các thuộc tính thực thể: thuộc tính, đa giá trị thuộc tính, thuộc tính tổng hợp, các thuộc tính phát sinh.
6. Xác định mối quan hệ giữa các entities
7. Sử dụng symbols để vẽ sơ đồ

![image](<Pictures_Source/Picture1.png>)

**Mối quan hệ**
- Derived Attributes: Thuộc tính không tồn tại trong db vật lý mà giá trị của nó được dẫn xuất từ các thuộc tính khác hiện hữu trong db
- Thực thể yếu: thực thể nằm rìa của db (có cũng được, không có cũng không sao), phải phụ thuộc vào thực thể mạnh.
- Xem sub-class trong sách
1. **Mỗi phòng ban có thể có nhiều địa điểm khác nhau. Mỗi địa điểm được phân công bởi nhiều phòng ban, địa điểm gồm mã: địa điểm, tên địa điểm.**
2. **Dự án có mã duy nhất, tên dự án do 1 phòng ban chủ trì và được triển khai ở 1 địa điểm.**

## Chuyển đổi từ ERD sang relation model
1. Mỗi entity tương ứng với mỗi relation
   Những attributes của từng entity tương ứng các relation của từng relation đ
   Thuộc tính nào của attribute là khóa chính của entity, đó cũng là khóa chính của relation đó
2. Tiến hành chuyển đổi dựa trên mối kêt hợp:
   - 1-M: lấy khóa chính của 1 thêm vào M
   - M-M: tạo ra 1 relation mới, tên của relation đó cũng là tên của relationship trong ERD. Khóa của relationship mới sẽ là khóa của 2 entity liên quan. Nếu relationship đó có attribute on relationship thì thêm relation mới luôn.
    - 1-1: Lấy khóa của entity này đẩy vào entity kia. Tuy nhiên ưu tiên bên nào có đầy đủ thành phần tham gia. Nếu có attribute on relationship thì đẩy vào theo hướng đẩy của khóa luôn
3. Trường hợp đặc biệt là thực thể yếu: lấy khóa của strong entity đẩy vào weak entity. Nhưng lưu ý: khóa chính của strong entity sẽ là khóa chính của weak entity sau khi đẩy vào luôn.
