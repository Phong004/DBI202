# Chapter 3
## Functional Dependency
- **Phụ thuộc hàm** là ràng buộc giữa 2 tập thuộc tính của một quan hệ.
- **Siêu khóa**: nếu L là siêu khóa, K là khóa, thì $$K\subseteq L$$
- **Tiên đề Amstrong**:
  1. Luật phản xạ: Nếu X là con của Y thì $$Y\rightarrow X$$
  2. Luật tăng trưởng: nếu $$X\rightarrow Y$$, thì $$XZ\rightarrow YZ$$
  3. Luật bắc cầu: nếu $$X\rightarrow Y$$ và $$Y\rightarrow Z$$, thì $$X\rightarrow Z$$

     **Luật suy rộng**:
  1. $$X\rightarrow Y\land X\rightarrow Z$$ then $$X\rightarrow YZ$$
  2. $$X\rightarrow YZ$$ then $$X\rightarrow Y\land X\rightarrow Z$$
  3. $$X\rightarrow \land WY\rightarrow Z$$ then $$WX\rightarrow Z$$
## Closure of Attributes
- Bao đóng của tập thuộc tính {$$A_1, A_2,..., A_n$$} nằm dưới S (ký hiệu $$\{A_1, A_2,... ,A\}^+$$ là tập thuộc tính B sao cho mỗi quan hệ thỏa mãn tất cả FD trong tập S cũng thỏa mãn $$A_1, A_2...A_n\rightarrow B$$
## Anomalies
![image](<Pictures_Source/Picture1.png>)
1. 1NF: 
