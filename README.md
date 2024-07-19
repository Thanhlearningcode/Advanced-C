**Lesson 3: POINTER**

Trong ngôn ngữ lập trình C, con trỏ (pointer) là một biến chứa địa chỉ bộ nhớ của một biến khác. Việc sử dụng con trỏ giúp chúng ta thực hiện các thao tác trên bộ nhớ một cách linh hoạt hơn.
Cách khai báo:      datatype * PointerName; 	

**A. Void Pointer**
Là một con trỏ đặc biệt có thể trỏ tới các đối tượng thuộc bất kỳ kiểu dữ liệu nào.
Cách khai báo:      void *PointerName; 

Ex:

![image](https://github.com/user-attachments/assets/2f983629-c064-408c-b717-b8f9b22d9594)

![image](https://github.com/user-attachments/assets/0f576021-96f4-4e89-986a-6753678b333f)

**C. Pointer to Constant**
Định nghĩa một con trỏ không thể thay đổi giá trị tại địa chỉ mà nó trỏ đến thông qua dereference nhưng giá trị tại địa chỉ đó có thể thay đổi.
Cách khai báo:     int const *ptr_const;
		     const int *ptr_const;
Ex:
![image](https://github.com/user-attachments/assets/e1e8ed18-4592-43d5-973d-fc7a8f98c8a5)

![image](https://github.com/user-attachments/assets/6d1434c0-6047-49ad-83c3-137fd579ad15)


**D. Constant Pointer**
Định nghĩa một con trỏ mà giá trị nó trỏ đến không thể thay đổi. 
Cách khai báo:     int *const const_ptr = &value;
Ex:

![image](https://github.com/user-attachments/assets/69d00873-f034-44b8-9a76-9ba0cfa0081d)

![image](https://github.com/user-attachments/assets/4eacf2a5-c0f8-479c-91d2-8a60fb588409)

**B. Function Pointer**
Là một biến mà giữ địa chỉ của một hàm, nó trỏ đến vùng nhớ trong bộ nhớ chứa mã máy của hàm được định nghĩa trong chương trình.
Cách khai báo:      <return_type>  (*<PointerName>)( <ParametersDataType> );
Ex:
![image](https://github.com/user-attachments/assets/77914c97-c518-4881-90a0-082f0df8b530)

![image](https://github.com/user-attachments/assets/555d5d2a-d4bd-4a0e-a31e-da696332cc9c)

**C. Pointer to Constant**
Định nghĩa một con trỏ không thể thay đổi giá trị tại địa chỉ mà nó trỏ đến thông qua dereference nhưng giá trị tại địa chỉ đó có thể thay đổi.
Cách khai báo:     int const *ptr_const;
		     const int *ptr_const;
Ex:
![image](https://github.com/user-attachments/assets/919b6f4f-44db-4a82-b136-71c0efdc07c2)
![image](https://github.com/user-attachments/assets/3a993a76-198c-4f3b-bc16-c0bfa1933fc2)

**D. Constant Pointer**
Định nghĩa một con trỏ mà giá trị nó trỏ đến không thể thay đổi. 
Cách khai báo:     int *const const_ptr = &value;
Ex:

![image](https://github.com/user-attachments/assets/e2471499-2f09-4856-bb82-481c0e71f156)
![image](https://github.com/user-attachments/assets/4355035e-2fb2-4e41-ab37-1afa7cf5a5e3)

**E. Pointer to Pointer**
Là kiểu dữ liệu trong ngôn ngữ lập trình cho phép lưu trữ địa chỉ của một con trỏ	
Cách khai báo: int *ptr = &test;
                             int **ptp = &ptr;
Ex:

![image](https://github.com/user-attachments/assets/5657b41b-6274-4051-9e97-73a0fa813469)
![image](https://github.com/user-attachments/assets/ac773ace-dbda-41d2-942f-e79c7598ffd8)


**F. NULL Pointer**

Là một con trỏ không trỏ đến bất kỳ đối tượng hoặc vùng nhớ cụ thể nào. Sử dụng null pointer thường hữu ích để kiểm tra xem một con trỏ đã được khởi tạo và có trỏ đến một vùng nhớ hợp lệ chưa.
Ex:


![image](https://github.com/user-attachments/assets/e403de60-f061-4ec9-ad6e-b35f7d42ff6e)

LESSON 5: GOTO + SETJMP

Goto: goto là một từ khóa trong ngôn ngữ lập trình C, cho phép chương trình nhảy đến một nhãn (label) đã được đặt trước đó trong cùng một hàm. Mặc dù nó cung cấp khả năng kiểm soát flow của chương trình, nhưng việc sử dụng goto thường được xem là không tốt vì nó có thể làm cho mã nguồn trở nên khó đọc và khó bảo trì.
![image](https://github.com/user-attachments/assets/20ba64a7-1c17-49b5-aeb2-796088e89650)

![image](https://github.com/user-attachments/assets/b34c2afc-ed2b-47dc-8d76-23b07e5c4f1f)

SETJMP :setjmp.h là một thư viện trong ngôn ngữ lập trình C, cung cấp hai hàm chính là setjmp và longjmp. Cả hai hàm này thường được sử dụng để thực hiện xử lý ngoại lệ trong C, mặc dù nó không phải là một cách tiêu biểu để xử lý ngoại lệ trong ngôn ngữ này.

![image](https://github.com/user-attachments/assets/663601f5-7608-45ab-8d24-177d8ab7284f)











