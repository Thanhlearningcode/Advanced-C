![image](https://github.com/user-attachments/assets/a480c3fc-b5ad-4868-87f7-9e386f1f7768)**Lesson 3: POINTER**

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

LESSON 4: GOTO + SETJMP

Goto: goto là một từ khóa trong ngôn ngữ lập trình C, cho phép chương trình nhảy đến một nhãn (label) đã được đặt trước đó trong cùng một hàm. Mặc dù nó cung cấp khả năng kiểm soát flow của chương trình, nhưng việc sử dụng goto thường được xem là không tốt vì nó có thể làm cho mã nguồn trở nên khó đọc và khó bảo trì.
![image](https://github.com/user-attachments/assets/20ba64a7-1c17-49b5-aeb2-796088e89650)

![image](https://github.com/user-attachments/assets/b34c2afc-ed2b-47dc-8d76-23b07e5c4f1f)

SETJMP :setjmp.h là một thư viện trong ngôn ngữ lập trình C, cung cấp hai hàm chính là setjmp và longjmp. Cả hai hàm này thường được sử dụng để thực hiện xử lý ngoại lệ trong C, mặc dù nó không phải là một cách tiêu biểu để xử lý ngoại lệ trong ngôn ngữ này.

![image](https://github.com/user-attachments/assets/663601f5-7608-45ab-8d24-177d8ab7284f)
Bài 5: Extern - Static - Volatile
Khái niệm extern trong ngôn ngữ lập trình C được sử dụng để thông báo rằng một biến hoặc hàm đã được định nghĩa ở một nơi khác trong chương trình hoặc trong một file nguồn khác. Khi sử dụng từ khóa extern, chúng ta cho trình biên dịch biết rằng biến hoặc hàm này đã được khai báo và định nghĩa ở một file khác, và chúng ta chỉ đang tham chiếu đến nó. Điều này giúp quản lý sự liên kết giữa các phần khác nhau của chương trình hoặc giữa các file nguồn một cách hiệu quả, cho phép chia sẻ biến và hàm giữa các file mà không cần phải định nghĩa lại chúng nhiều lần
#include <stdio.h>

extern int count; // Tham chiếu đến biến count được khai báo ở file khác

void displayCount();

int main() {
    count = 5;
    displayCount();
    return 0;
}
#include <stdio.h>

int count; // Định nghĩa biến count

void displayCount() {
    printf("Count: %d\n", count);
}
Static local variables
**Static** được sử dụng với biến cục bộ (biến được khai báo trong một hàm) trong ngôn ngữ lập trình C, nó có các đặc điểm sau:

Giữ giá trị qua các lần gọi hàm: Biến cục bộ static giữ giá trị của nó giữa các lần gọi hàm, không bị khởi tạo lại mỗi khi hàm được gọi. Điều này có nghĩa là giá trị của biến sẽ được bảo toàn qua các lần thực thi hàm.

Phạm vi chỉ trong hàm: Phạm vi của biến cục bộ static vẫn chỉ giới hạn trong hàm nơi nó được khai báo. Biến không thể được truy cập từ bên ngoài hàm.
Static global variables
**STATIC** được sử dụng với biến toàn cục (biến được khai báo bên ngoài tất cả các hàm) trong ngôn ngữ lập trình C, nó có các đặc điểm sau:

Phạm vi chỉ trong file nguồn hiện tại: Biến toàn cục static bị giới hạn phạm vi trong file nguồn mà nó được khai báo. Điều này có nghĩa là biến này không thể được truy cập từ các file nguồn khác trong cùng một chương trình. Nó giúp tránh xung đột tên biến khi các file nguồn khác nhau sử dụng cùng một tên biến.

Ứng dụng: Biến toàn cục static thường được sử dụng trong các file thư viện để ẩn các biến khỏi các file nguồn khác, giúp tránh việc truy cập ngoài ý muốn và tăng tính đóng gói của mã nguồn.
Volatile
Từ khóa volatile trong ngôn ngữ lập trình C được sử dụng để báo hiệu cho trình biên dịch rằng một biến có thể thay đổi ngẫu nhiên, ngoài sự kiểm soát của chương trình. Việc này ngăn chặn trình biên dịch tối ưu hóa hoặc xóa bỏ các thao tác trên biến đó, giữ cho các thao tác trên biến được thực hiện như đã được định nghĩa.
- Thường sẽ ứng dụng trong UART *data, ngắt....
BIT MASK
I. Khái niệm
Bitmask là một kỹ thuật sử dụng các bit để lưu trữ và thao tác để biểu diễn trạng thái cho nhiều đối tượng.
Bitmask thường được sử dụng để tối ưu hóa bộ nhớ, thực hiện các phép toán logic trên một cụm bit hoặc các thuộc tính khác của một đối tượng.
II. Các toán tử BitWise
a, BitWise AND &
Thực hiện phép AND giữa từng bit của hai số. Nếu hai bit tương ứng đều là 1 thì kết quả là 1, ngược lại thì kết quả là 0.
Ex:
  
 
b, BitWise OR (|)
Thực hiện phép OR giữa từng bit của hai số. Nếu có hơn một trong hai bit có giá trị là 1 thì kết quả là 1.
Ex:
 ![image](https://github.com/user-attachments/assets/ef9e5ff6-1bcf-4e16-a3f5-606ee8461fdc)
![image](https://github.com/user-attachments/assets/ad10591d-171d-4c6a-860a-40e3b2f7e3a0)

  
c, BitWise XOR (^)
Thực hiện phép XOR giữa từng bit của hai số. Nếu chỉ một trong hai bit có giá trị là 1 thì kết quả là 1.
Ex:
 ![image](https://github.com/user-attachments/assets/ff73dab2-bf8b-43c1-aeee-6614508d656f)
![image](https://github.com/user-attachments/assets/9e70639d-7a01-423e-ae65-5b8e2a6a7165)

 
d, NOT bitwise
Thực hiện phép NOT bitwise trên từng bit của một số. Kết quả là bit đảo ngược của số đó.
Ex:
 ![image](https://github.com/user-attachments/assets/86eadb30-d9b9-45a5-b61e-69ba451cf392)
![image](https://github.com/user-attachments/assets/572d227c-a4ef-4151-a4e2-fc4cbc3edbdd)

 
Struct – Union
1. Struct
Struct là một kiểu dữ liệu bao gồm nhiều thành phần có thể thuộc nhiều kiểu dữ liệu khác nhau. Struct cho phép tạo ra một thực thể dữ liệu lớn hơn và có tổ chức hơn từ các thành viên (members) của nó.
Cú pháp:
![image](https://github.com/user-attachments/assets/39aa94fd-2e51-4942-9ea6-c80cb577b65e)
Mỗi biến trong Struct được gọi là thành phần và để truy cập các thành phần thì bạn có thể sử dụng toán tử ( . )
Con trỏ tới Struct khai báo bằng cách đặt dấu * trước tên của struct, toán tử -> được sử dụng để truy cập vào các phần tử của một struct khi đó là con trỏ. Con trỏ struct cho phép thay đổi trực tiếp phần tử của struct
![image](https://github.com/user-attachments/assets/51d7a56b-71dc-4cfb-ab53-1930fd4fc49e)
2. Union
Union là một cấu trúc dữ liệu kết hợp nhiều kiểu dữ liệu khác nhau vào một cùng một vùng nhớ. Nhưng chỉ có thể truy cập một giá trị trong union tại một thời điểm, kích thước của union bằng với kích thước của thành viên lớn nhất.
Cú pháp:
![image](https://github.com/user-attachments/assets/ff04db52-9c4c-4d54-8870-51bfa3cc9ac1)
3. Sự khác nhau giữa Struct và Union
Struct:
•	Mỗi thành phần trong struct có địa chỉ riêng và chiếm không gian riêng trong bộ nhớ.
•	Dung lượng bộ nhớ của struct bằng tổng dung lượng của tất cả các thành phần trong struct.
•	Khi truy cập các thành phần của struct, có thể truy cập độc lập vào từng thành phần.
Cách tính dung lượng bộ nhớ struct:
•	Đầu tiên trình biên dịch sẽ lấy kích thước của trường dữ liệu thành phần có kích thước lớn nhất
•	Sau đó cấp phát 1 block gồm đúng bằng kích thước này 
•	Thành phần được khai báo đầu tiên trong struct sẽ ở vị trí đầu tiên trong bộ nhớ
![image](https://github.com/user-attachments/assets/5f75b9b0-b474-4dd5-b6ee-633e0eee23e0)
•	Sau đó tiếp tục đẩy thành phần tiếp theo vào trong bộ nhớ. Ở đây thành phần age có kích thước 4 bytes, có thể hiểu để analysis n byte thì ở trước đó cần analysis n byte trước vì vậy khi cấp phát bộ nhớ cho age thì trình biên dịch sẽ tự động tạo thêm 3 bytes để analysis đủ 4 byte.
![image](https://github.com/user-attachments/assets/e39428e1-1ccc-4d47-bfad-e7fd3cfd35bc)
Union:
•	Dung lượng bộ nhớ của một biến union bằng với dung lượng của thành phần lớn nhất trong union.
•	Tất cả các thành phần của union chia sẽ cùng một vùng nhớ, do đó khi gán giá trị cho một thành phần, giá trị của thành phần khác sẽ bị thay đổi.




