# Advanced C
**Lesson 3: POINTER**

What is Pointer?
- In the C programming language, a pointer is a variable that holds the memory address of another variable. The use of pointers allows us to perform operations on memory in a more flexible way. Here are some basic concepts about pointers in C:
  + **Khai báo con trỏ**: Con trỏ được khai báo bằng cách sử dụng ký hiệu dấu sao (*) và chỉ ra rằng biến đó là một con trỏ đến một kiểu dữ liệu nhất định.Exp: int *ptr;
  + **Khởi tạo con trỏ**: Con trỏ phải được khởi tạo bằng cách gán địa chỉ của một biến cho nó, thường là bằng toán tử địa chỉ (&). Exp: int &a; ( 0x01 address)
  + **Con trỏ và mảng**: Trong C, tên mảng đóng vai trò như một con trỏ đến phần tử đầu tiên của mảng đó, thiết lập mối quan hệ chặt chẽ giữa mảng và con trỏ.
    Exp:
 ![image](https://github.com/user-attachments/assets/443fbf09-0e1e-4917-aa28-361cff156d48)


  +  **Con trỏ null:** Con trỏ null là một giá trị đặc biệt chỉ ra rằng con trỏ không trỏ tới bất kỳ vị trí bộ nhớ hợp lệ nào.
    EXP(quan trọng ): Giả sử không dùng free,smartpointer làm sao để thu hồi con trỏ đã cấp phát???? ->>> Int a=1;
                                                                                                          int *ptr =a;
                                                                                                          ptr=NULL;// Thu hồi con trỏ
  + **Con trỏ đến con trỏ**: Con trỏ có thể trỏ tới các con trỏ khác, tạo ra nhiều cấp độ gián tiếp, có ích trong các kịch bản lập trình phức tạp.
  ![image](https://github.com/user-attachments/assets/e0f86989-94ae-4f03-9e79-6367971c52f5)

  + Pointer to Constant: Đây là một loại con trỏ trong C mà không thể thay đổi giá trị của biến mà nó trỏ đến thông qua dereference (toán tử *), nhưng giá trị của biến đó có thể thay đổi bằng các phương thức khác (ví dụ: gán trực tiếp).
![image](https://github.com/user-attachments/assets/c5cfa98c-f73a-404a-b8f2-1d31fa460daa)

  ![image](https://github.com/user-attachments/assets/a643507c-8a6b-4c9b-872f-0440e7051040)





      
                                                                                                          
