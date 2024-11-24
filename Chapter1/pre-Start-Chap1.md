# The Worlds of Database Systems
## 1. The Evolution of Database Systems
**Data** là các **sự kiện** *<ins>thô sơ</ins>*, *<ins>không có cấu trúc</ins>* cần được xử lý để làm cho nó có ý nghĩa. **Data** có thể được xem như là các *sự kiện* và *thống kê* được thu thập cùng nhau nhằm phục vụ cho việc tham khảo hoặc phân tích.
**Có 2 loại data**
  1. Quantitative (Định lượng): thông tin dạng số như chiều cao, cân nặng,...
  2. Qualitative (Định tính): thông tin không phải là số như các ý kiến, nhận thức,...

**Information** là dữ liệu (**Data**) *<ins>có cấu trúc</ins>*, *<ins>có tổ chức</ins>*, *<ins>đã được xử lý</ins>*, được biểu diễn trong một ngữ cảnh cụ thể liên quan và có ích với người cần nó.
<table>
    <thead>
        <tr>
            <th><span>S.NO</span></th>
            <th><span>DATA</span></th>
            <th><span>INFORMATION</span></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>
                <p dir="ltr"><span>Definition</span></p>
            </th>
            <td>
                <p dir="ltr"><span>Data is defined as unstructured information such as text, observations, images, symbols, and descriptions. In other words, data provides no specific function and has no meaning on its own. </span></p>
            </td>
            <td>
                <p dir="ltr"><span>Information refers to processed, organized, and structured data. It gives context for the facts and facilitates decision making. In other words, information is processed data that makes sense to us. </span></p>
            </td>
        </tr>
        <tr>
            <th><b><strong>Purpose</strong></b></th>
            <td><span>Data are the variables that help to develop ideas/conclusions.</span></td>
            <td><span>Information is meaningful data.</span></td>
        </tr>
        <tr>
            <th><b><strong>Natur</strong></b><span>e</span></th>
            <td><span>Data are text and numerical values.</span></td>
            <td><span>Information is refined form of actual data.</span></td>
        </tr>
        <tr>
            <th><b><strong>Dependence</strong></b></th>
            <td><span>Data doesn’t rely on Information.</span></td>
            <td><span>While Information relies on Data.</span></td>
        </tr>
        <tr>
            <th><b><strong>Measurement</strong></b></th>
            <td><span>Bits and Bytes are the measuring unit of data.</span></td>
            <td><span>Information is measured in meaningful units like time, quantity, etc.</span></td>
        </tr>
        <tr>
            <th><b><strong>Structure</strong></b></th>
            <td><span>As tabular data, graphs, and data trees can be easily structured.</span></td>
            <td><span>Information can also be structured as language, ideas, and thoughts.</span></td>
        </tr>
        <tr>
            <th><b><strong>Purposefulness</strong></b></th>
            <td><span>Data does not have any specific purpose</span></td>
            <td><span>Information carries a meaning that has been assigned by interpreting data.</span></td>
        </tr>
        <tr>
            <th><b><strong>Knowledge Level</strong></b></th>
            <td><span>It is low-level knowledge.</span></td>
            <td><span>It is the second level of knowledge.</span></td>
        </tr>
        <tr>
            <th><b><strong>Decision Making</strong></b></th>
            <td><span>Data does not directly help in decision making.</span></td>
            <td><span>Information directly helps in decision making.</span></td>
        </tr>
        <tr>
            <th><b><strong>Meaning</strong></b></th>
            <td><span>Data is a collection of facts, which itself has no meaning.</span></td>
            <td><span>Information puts those facts into context.</span></td>
        </tr>
        <tr>
            <th><b><strong>Example</strong></b></th>
            <td><span>Example of data is student test scores.</span></td>
            <td><span>Example of information is average score of class that is derived from given data.</span></td>
        </tr>
    </tbody>
</table>

 __${\color{red}Database}$ - Cơ sở dữ liệu__
 - Một bộ các thông tin tồn tại qua một thời gian dài.
 - Bộ các dữ liệu liên quan nhau.
 - Quản lý bằng DBMS - Database Management System

__${\color{red}DBMS}$ - Hệ quản lý cơ sở dữ liệu__
- Là phần mềm có chức năng tạo và bảo trì một hệ cơ sở dữ liệu tính toán.

__${\color{red}Database\space System}$__
- Phần mêm *DBMS* cùng với *Data*, đôi khi còn bao gồm các ứng dụng.

![image](<Pictures_Source/Picture1.png>)

**DBMS** được trông đợi:
  1. Cho phép người dùng tạo mới cơ sở dữ liệu và chỉ định lược đồ của nó.
  2. Cho người dùng khả năng truy vấn dữ liệu
  3. Hỗ trợ lưu trữ lượng rất lớn cơ sở dữ liệu.
  4. Enable Durability
  5. Kiểm soát truy cập tới dữ liệu từ nhiều người dùng một lần.

**Early DBMS**: 1960s, the first DBMS based on file system
|Responsibility|Yes/No|
|:------------:|:-----|
|(1)|Limited|
|(2)|Not directly supported|
|(3)|Yes|
|(4)|Not always supported|
(5)|No|

**Cấu trúc cây phân cấp dữ liệu**
![image](<Pictures_Source/Picture3.png>)

**Cấu trúc đồ thị mạng dữ liệu** cho phép mỗi bản ghi có nhiều bản ghi cha hoặc nhiều bản ghi con.
$$\color{red}\rightarrow\space Không\space hỗ\space trợ\space truy\space vấn\space ngôn\space ngữ\space bặc\space cao$$

![image](<Pictures_Source/Picture2.png>)
![image](<Picture_Source/Picture4.png>)

**Smaller and Smaller System**
- DBMS vốn là phần mềm rất nặng và mắc chạy trên các máy tính lớn nhưng ngày nay nó đã có thể chạy trên PC, Mobile,...

=> Hệ cơ sở dữ liệu dựa trên mô hình quan hệ có sẵn cho các máy rất nhỏ.
**Bigger and Bigger System**
- Kích cỡ của dữ liệu được tăng liên tục
- Nhiều cơ sở dữ liệu lưu trữ hàng petabytes và phục vụ cho tất cả người dùng.
**Information Integration**
<Thiếu>
## 2. Overview of DBMS
**Database Management System**
<Thiếu>
**DBMS components**
<Thiếu>
**Database Users**
<Thiếu>
**DDL - Data Definition Language Commands**
<Thiếu>
**1. Trả lời truy vấn**
<Thiếu>
**2. Xử lý giao dịch**
<Thiếu>
**Xu hướng thiết kế DB và DBMS**
