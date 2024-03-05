# Size-of-Pointer-in-C

Như khi ta học lập trình thì kích thước của từng loại kiểu dữ liệu được ghi rõ trong bảng dưới đây.
<p align="center">
    <img src="./Images/value_structure.jpg" width="500px" alt="">
</p>

Khi nói đến hệ thống máy tính `32-bit` hay `64-bit` nghĩa là muốn nói đến `số bit` có thể được `xử lý đồng thời` bởi bộ xử lí - processor (CPU) của hệ thống máy tính đó.

**Problem:** *Có khi nào bạn tự hỏi liệu rằng kích thước của 1 con trỏ trong C là bao nhiêu hay không ?* 

Pointer in C is just a variable that could store the address of the other variable. In C size of a pointer is not fixed as it depends on Word size of the processor. In general a 32-bit computer machine then size of a pointer would be 4 bytes while for a 64-bit computer machine, it would be 8 bytes.

Ta biết được `con trỏ dùng để lưu trữ địa chỉ` của 1 `biến` nào đó. 
- Lấy ví dụ về 32-bit computer machine:
Thì nó sẽ có địa chỉ `memory` từ: 0x0000 0000 cho đến 0xFFFF FFFF. (Mỗi con số 0 tương ứng với 4-bit: 0 0 0 0) => Ở đây có 8 con số 0 là 32-bit.

Ảnh minh họa:
<p align="center">
    <img src="./Images/memory_image.png" width="500px" alt="">
</p>

Khi ta khai báo 1 biến bất kì thì nó sẽ được lưu trữ tại 1 vị trí trong bộ nhớ máy tính. (Địa chỉ của biến này nằm trong khoảng 0x0000 0000 -> 0xFFFF FFFF).

Giả sử: 
- Khai báo: int A = 5 => địa chỉ của biến A là 0x0061 FF0C.
- 
