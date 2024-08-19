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
  Bài 7 : BIT MASK
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

 Bài 8:
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
   Bài 9:
Memory Layout
Trong ngôn ngữ lập trình C, bộ nhớ của chương trình thường được phân chia thành các phân vùng khác nhau, mỗi phân vùng có mục đích và quy tắc sử dụng riêng.

 ![image](https://github.com/user-attachments/assets/9c3e1a02-1f5d-450a-a57c-7e9c1a6fe0ef)

1. Text Segment
•	Chứa code của chương trình.
•	Quyền truy cập: có quyền đọc nhưng không có quyền ghi.
•	Kích thước của Text Segment thường là cố định khi chương trình được biên dịch.
2. Data Segment
•	Chứa các biến global, static được tạo ra bởi lập trình viên.
•	Quyền truy cập: có quyền đọc và ghi.
3. BSS
•	Chứa các biến global, static được tạo ra bởi lập trình viên nhưng chưa có giá trị ban đầu.
•	Dữ liệu trong phân vùng này thường được xác định bởi giá trị 0.
•	Quyền truy cập: có quyền đọc và ghi.


 
Bài 10:

4. Heap
Được sử dụng để cấp phát bộ nhớ động, các biến được cấp phát trên heap không có kích thước xác định tại thời điểm biên dịch và có thể được quản lý động trong quá trình thực thi của chương trình.
•	Quyền truy cập: có quyền đọc và ghi.
•	Cấp Phát và Giải Phóng Bộ Nhớ: Các hàm như malloc(), calloc(), realloc(), và free()
•	Kích Thước Thay Đổi: Kích thước của heap có thể thay đổi trong quá trình thực thi của chương trình
•	Dữ liệu trong Heap sẽ không bị hủy khi hàm thực hiện xong, điều đó có nghĩa bạn phải tự tay giải phóng vùng nhớ bằng câu lệnh free

![image](https://github.com/user-attachments/assets/6fc1f6b4-6709-4a21-931f-727dfe0857f8)

5. Stack
Nó được sử dụng để lưu trữ các biến cục bộ, các giá trị trả về từ hàm, địa chỉ trả về và một số thông tin khác liên quan đến thực thi của chương trình.
Đặc điểm:
•	Stack hoạt động theo nguyên tắc LIFO
•	Kích thước của stack là cố định vì vậy khi khởi tạo quá nhiều biến cục bộ, đệ quy thì có thể sảy ra hiện tượng overflow
•	Khi một hàm được gọi, các giá trị và địa chỉ trong hàm đó được đẩy vào Stack. Sau khi hàm kết thúc, những giá trị này được lấy ra để quay trở lại thực thi chương trình.
#include <stdio.h>

![image](https://github.com/user-attachments/assets/3546adce-a394-4088-aeea-1c0ca0f29744)
Bài 11:
JSION
JSION Là một định dạng truyền tải dữ liệu phổ biến trong lập trình và giao tiếp giữa các máy chủ và trình duyệt web, cũng như giữa các hệ thống khác nhau.
JSION Sử dụng một cú pháp nhẹ dựa trên cặp khóa-giá trị, tương tự như các đối tượng và mảng trong JavaScript. Mỗi đối tượng JSON bao gồm một tập hợp các cặp "key" và "value", trong khi mỗi mảng JSON là một tập hợp các giá trị.
1. Định dạng của JSION
a, Kiểu dữ liệu
•	Null
•	Boolean: true hoặc false.
•	Number: Có thể là số nguyên hoặc số thập phân.
•	String: Chuỗi ký tự, được bao bọc bởi dấu nháy đơn ('') hoặc nháy kép ("").
•	Array: danh sách các giá trị, giữa mỗi giá trị sử dụng dấu phẩy.
•	Object: Một tập hợp các cặp key - value, giữa mỗi cặp sử dụng dấu hai chấm (:). Đối tượng được bao bọc bởi dấu ngoặc nhọn ({}).
b, Key – Value
Mỗi cặp key(string) - value được phân tách bằng dấu : và mỗi cặp key – value được ngăn cách bằng dấu ,
Ví dụ:
{
    "name" : "Nguyen Van Thanh",	
    "age" : 18,	
    "SID": 101210075,	
    "Score" : [9.2, 10, 8.5]
}

Bài 11 :
Linked List
Linked list được sử dụng để tổ chức và lưu trữ dữ liệu. Một linked list bao gồm một chuỗi các "nút", mỗi nút chứa một giá trị dữ liệu và một con trỏ đến nút tiếp theo trong chuỗi.
Phần tử cuối cùng trong DSLK trỏ đến NULL  
![image](https://github.com/user-attachments/assets/4256010c-ca82-484f-ae78-6b24eae2bdd4)

Đặc điểm:
•	Tiết kiếm bộ nhớ và cấp phát động
•	Có thể lưu các phần tử ở bất cứ đâu được phép trên bộ nhớ
•	Dễ dàng insert và delete
Có 2 loại Linked list:
•	Singly Linked List: Mỗi nút chỉ chứa một con trỏ đến nút tiếp theo trong chuỗi.
•	Doubly Linked List (Danh sách liên kết đôi): Mỗi nút chứa hai con trỏ, một trỏ đến nút tiếp theo và một trỏ đến nút trước đó.
Cấu trúc một Node: 
![image](https://github.com/user-attachments/assets/9c79b267-32a5-48b4-8a15-ff390faad1a6)

Các quy tắc về đặt tên theo tiêu chuẩn “Autosar C Coding Guidelines”
Tiêu Chuẩn C
“Autosar C Coding Guidelines” là một trong những tiêu chuẩn phổ biến được sử dụng trong lĩnh vực phát triển các hệ thống nhúng. Tiêu chuẩn này cung cấp các quy tắc và hướng dẫn cho việc viết code theo chuẩn Autosar C, giúp đảm bảo tính linh hoạt, dễ bảo trì và dễ mở rộng của hệ thống nhúng.

    Tiêu chuẩn Autosar C Coding Guidelines bao gồm nhiều quy tắc về đặt tên biến và hàm, sử dụng hằng số, định dạng code, sử dụng comment, kiểm tra mã nguồn, v.v. Quy tắc này được thiết kế để đảm bảo rằng các nhà phát triển có thể viết code đồng nhất và dễ đọc, giúp giảm thiểu lỗi và tăng tính ổn định của hệ thống nhúng.

    Ngoài ra, tiêu chuẩn Autosar C Coding Guidelines cũng đưa ra các hướng dẫn về việc sử dụng các công cụ phân tích mã nguồn để tìm lỗi và cải thiện tính năng của hệ thống nhúng. Điều này là cực kỳ quan trọng đối với các hệ thống nhúng có tính chính xác cao và độ tin cậy yêu cầu cao, như trong các hệ thống điều khiển động cơ và hệ thống an toàn.

    Tóm lại, tiêu chuẩn Autosar C Coding Guidelines là một chuẩn mực quan trọng cho việc viết code trong lĩnh vực Autosar C. Việc tuân thủ tiêu chuẩn này giúp đảm bảo tính linh hoạt, dễ bảo trì và dễ mở rộng của hệ thống nhúng, đồng thời giảm thiểu lỗi và tăng tính ổn định của hệ thống nhúng.

    Dưới đây là danh sách tất cả các quy tắc trong tiêu chuẩn Autosar C Coding Guidelines:

1. Quy tắc chung

– Sử dụng tên biến, hằng số, hàm và cấu trúc có ý nghĩa. Tên của chúng nên phản ánh chính xác chức năng và mục đích của chúng.

– Sử dụng các biến cục bộ để giảm thiểu phạm vi của chúng. Biến toàn cục nên được sử dụng chỉ khi cần thiết và không thể thay thế bằng biến cục bộ.

– Sử dụng các hằng số để định nghĩa các giá trị không thay đổi trong chương trình.

– Khai báo các biến ở đầu của khối mã. Nếu có thể, hãy khai báo và gán giá trị ban đầu cho biến cùng lúc.

– Sử dụng các toán tử và hàm thư viện chuẩn của ngôn ngữ để tránh việc viết lại các phép tính hoặc hàm đã có sẵn.

– Sử dụng các lệnh điều kiện và vòng lặp một cách cẩn thận và đảm bảo chúng đúng về mặt logic và hiệu năng.

– Đối với các hàm, nên tránh sử dụng quá nhiều tham số. Nếu số lượng tham số quá lớn, hãy sử dụng các cấu trúc để truyền các giá trị.

– Sử dụng cấu trúc dữ liệu và lớp đối tượng để tổ chức mã của bạn. Các cấu trúc dữ liệu và lớp đối tượng nên được thiết kế sao cho có tính đóng gói và tránh việc truy cập trực tiếp vào các thành phần bên trong.

– Sử dụng comment để giải thích mã của bạn, đặc biệt là những phần mã khó hiểu hoặc dễ bị lỗi.

– Sử dụng kiểu dữ liệu phù hợp cho từng giá trị, tránh sử dụng kiểu dữ liệu không cần thiết hoặc không an toàn.

– Kiểm tra lỗi và xử lý ngoại lệ một cách chính xác và cẩn thận.

2. Quy tắc về đặt tên

– Sử dụng tên biến, hằng số, hàm và cấu trúc có ý nghĩa. Tên của chúng nên phản ánh chính xác chức năng và mục đích của chúng.

– Sử dụng các từ viết tắt chỉ khi cần thiết và đảm bảo rằng chúng được giải thích rõ ràng và hiểu được bởi mọi người.

– Sử dụng kiểu đặt tên theo kiểu CamelCase cho các biến và hàm.

– Sử dụng kiểu đặt tên theo kiểu PascalCase cho các cấu trúc và lớp đối tượng.

– Sử dụng chữ hoa cho các hằng số.

– Sử dụng các từ khóa đặc biệt như “const” hoặc “static” để làm rõ rằng biến là hằng số hoặc cục bộ.

– Đặt tên các biến theo quy tắc “type + name” để biểu thị kiểu dữ liệu của biến.

– Đặt tên các biến trong hàm theo quy tắc “type + name” hoặc “name + type” để biểu thị kiểu dữ liệu của biến và thứ tự truyền vào. 

– Sử dụng các tên biến dễ hiểu và ít gây nhầm lẫn. Ví dụ: không nên sử dụng các tên như “x”, “y” hoặc “temp” để đại diện cho các biến.

Dưới đây là các ví dụ về các quy tắc đặt tên trong Autosar C Coding Guidelines:

Sử dụng kiểu đặt tên CamelCase cho biến và hàm:

int numCars = 10;
float totalSales = 1000.0;
void getVehicleInfo() { ... }
Sử dụng kiểu đặt tên PascalCase cho các cấu trúc và lớp đối tượng:

struct CarModel { ... };
class SalesReport { ... };
Sử dụng chữ hoa cho các hằng số:

const int MAX_NUM_CARS = 100;
const float DEFAULT_SPEED_LIMIT = 60.0;
Đặt tên biến theo quy tắc “type + name”:

int iNumCars = 10;
float fSalesTotal = 1000.0;
Đặt tên biến trong hàm theo quy tắc “type + name” hoặc “name + type”:

int calculateRevenue(int iNumCars, float fPricePerCar);
void printSalesReport(SalesReport rptSales);
Sử dụng tiền tố cho biến để chỉ định mục đích sử dụng của biến:

int g_iNumCars = 10; // biến toàn cục
int s_iSalesTotal = 1000.0; // biến cục bộ tĩnh
Đặt tên hàm để thể hiện mục đích và hoạt động của nó:

int calculateRevenue(int iNumCars, float fPricePerCar); // tính doanh thu
void printSalesReport(SalesReport rptSales); // in báo cáo doanh số
Đặt tên hàm callback để thể hiện mục đích và cách sử dụng của nó:

void ButtonClickedCallback(void); // callback được gọi khi nút được nhấn
Đặt tên enum và các hằng số để thể hiện ý nghĩa của chúng:

enum CarType { SEDAN, SUV, SPORTS };
const int MAX_NUM_SEATS = 8;
Đặt tên các file và thư mục để thể hiện nội dung của chúng:

car_model.h // khai báo cấu trúc thông tin xe
sales_report.cpp // mã nguồn tính toán báo cáo doanh số
3. Quy tắc về comment

– Block-level comment: là một loại comment được đặt ở đầu của một phạm vi code, chẳng hạn như một file, một module hoặc một class, và được sử dụng để cung cấp thông tin về mục đích, tác giả, ngày tạo và các thông tin khác về phạm vi code đó.

    Trong ngôn ngữ lập trình C, block-level comment được đặt bắt đầu bằng ký hiệu /* và kết thúc bằng ký hiệu */, và nội dung của comment được đặt giữa hai ký hiệu này.

    Ví dụ:

/*
* File: sample_file.c
* Author: John Doe
* Date: 24/03/2023
* Description: This is a sample file for demonstrating block-level comment
*/
    Trong ví dụ trên, block-level comment được sử dụng để cung cấp thông tin về tên file, tác giả, ngày tạo và mô tả cho file “sample_file.c”. Khi đọc code, các lập trình viên khác có thể dễ dàng hiểu được thông tin về phạm vi code này và sử dụng nó đúng cách.

– Function-level comment: là một loại comment được đặt trước một hàm và được sử dụng để cung cấp thông tin về tên, mô tả, tham số và giá trị trả về của hàm đó. Function-level comment giúp các lập trình viên hiểu rõ hơn về chức năng của hàm và cách sử dụng nó trong code.

    Trong ngôn ngữ lập trình C, function-level comment được đặt trên một dòng riêng biệt và bắt đầu bằng ký hiệu /* và kết thúc bằng ký hiệu */. Nội dung của function-level comment bao gồm các thông tin sau:

+ Tên hàm

+ Mô tả về chức năng của hàm

+ Các tham số và kiểu dữ liệu của chúng

+ Giá trị trả về của hàm (nếu có)

    Ví dụ:

/*
* Function: calculate_sum
* Description: This function calculates the sum of two integers
* Input:
*   a - an integer value
*   b - an integer value
* Output:
*   returns the sum of a and b
*/
int calculate_sum(int a, int b) {
  return a + b;
}
    Trong ví dụ trên, function-level comment được sử dụng để cung cấp thông tin về tên hàm, chức năng của hàm là tính tổng của hai số nguyên, kiểu và tên của các tham số, và giá trị trả về của hàm. Các lập trình viên khác có thể dễ dàng hiểu được cách sử dụng hàm này trong code.

4. Quy tắc về xử lý lỗi

Không nên sử dụng goto để xử lý lỗi, thay vào đó sử dụng các cấu trúc điều kiện if-else hoặc switch-case để xử lý lỗi:

    Ví dụ:

// Không tốt
int process_data(int data) {
    int result = 0;
    if (data < 0) {
        goto error;
    }
    result = data * 2;
    return result;
error:
    return -1;
}
// Tốt
int process_data(int data) {
    if (data < 0) {
        return -1;
    }
    int result = data * 2;
    return result;
}
Sử dụng các hằng số để đại diện cho mã lỗi thay vì sử dụng các số cứng:

    Ví dụ:

/ Không tốt
int open_file() {
    FILE* fp = fopen("file.txt", "r");
    if (fp == NULL) {
        return -1;
    }
    return 0;
}
// Tốt
#define FILE_OPEN_FAILED -1
int open_file() {
    FILE* fp = fopen("file.txt", "r");
    if (fp == NULL) {
        return FILE_OPEN_FAILED;
    }
    return 0;
}
Sử dụng các hàm xử lý lỗi chuẩn như perror() hoặc strerror() để in ra thông báo lỗi:

    Ví dụ:

// Không tốt
void process_data() {
    int result = some_function();
    if (result == -1) {
        printf("Error: Some error occurred\n");
    }
}
// Tốt
void process_data() {
    int result = some_function();
    if (result == -1) {
        perror("Error");
    }
}
    Tóm lại, các quy tắc xử lý lỗi trong tiêu chuẩn Autosar C Coding Guidelines nhằm giúp người lập trình viết mã sạch và dễ bảo trì bằng cách tránh sử dụng các cấu trúc không tối ưu và sử dụng các cơ chế xử lý lỗi chuẩn một cách hiệu quả.

5. Quy tắc về định dạng code

    Định dạng code giúp cho code dễ đọc hơn, dễ hiểu hơn và dễ bảo trì hơn. Dưới đây là một số quy tắc định dạng code trong tiêu chuẩn Autosar C Coding Guidelines và ví dụ minh họa:

Khoảng trắng và dòng trống: sử dụng khoảng trắng và dòng trống để tạo ra các nhóm liên quan trong code. Để code dễ đọc hơn, hãy đặt dòng trống trước và sau các khối lệnh, đoạn mã, hàm, v.v.

    Ví dụ:

if (condition) {
    // code here
}
Thụt đầu dòng: sử dụng thụt đầu dòng để chỉ ra các phạm vi liên quan trong code. Thụt đầu dòng bằng 4 khoảng trắng. Ví dụ:

void example_function() {
    if (condition) {
        // code here
    } else {
        // code here
    }
}
Khoảng trắng trong phép toán: sử dụng khoảng trắng trong các phép toán để làm cho code dễ đọc hơn. Ví dụ:

int result = num1 + num2;
Khoảng trắng trong đối số và tham số hàm: sử dụng khoảng trắng để ngăn cách giữa các đối số và tham số trong hàm. Ví dụ:

void example_function(int arg1, float arg2, char arg3) {
    // code here
}
Chiều dài dòng: giới hạn độ dài của dòng code không quá 80 ký tự. Nếu một dòng code dài hơn 80 ký tự, hãy chia thành nhiều dòng. Ví dụ:

void example_function(int arg1, float arg2, char arg3) {
    if (arg1 > 0 && arg2 < 10.0 && arg3 == 'A') {
        // code here
    }
}
6. Quy tắc về sử dụng bộ nhớ

Không sử dụng con trỏ NULL: Tránh sử dụng con trỏ NULL trong ứng dụng vì nó có thể dẫn đến lỗi runtime hoặc crash hệ thống. Thay vào đó, nên sử dụng con trỏ hợp lệ và kiểm tra điều kiện để đảm bảo rằng chúng được sử dụng một cách an toàn.

    Ví dụ:

// Không nên sử dụng con trỏ NULL
int *ptr = NULL;
// Thay vào đó, nên sử dụng con trỏ hợp lệ
int num = 10;
int *ptr = &num;
Sử dụng kích thước phù hợp cho kiểu dữ liệu: Khi khai báo biến hoặc cấp phát bộ nhớ cho một đối tượng, cần sử dụng kích thước phù hợp với kiểu dữ liệu. Việc này giúp tiết kiệm bộ nhớ và đảm bảo an toàn khi thao tác với đối tượng đó.

    Ví dụ:

// Khai báo một mảng số nguyên với 10 phần tử
int arr[10];
// Cấp phát bộ nhớ cho một chuỗi ký tự với độ dài 20
char *str = malloc(20 * sizeof(char));
Sử dụng các phép toán bit thích hợp: Sử dụng các phép toán bit thích hợp để thực hiện các thao tác trên bit. Các phép toán bit như AND, OR, XOR, SHIFT được sử dụng rộng rãi trong lập trình nhúng để tiết kiệm bộ nhớ và tăng hiệu suất.

    Ví dụ:

// Sử dụng phép toán AND để kiểm tra bit thứ 2 của biến num
int num = 5;
if (num & (1 << 2)) {
    printf("Bit 2 of num is set\n");
}
// Sử dụng phép toán SHIFT để tính toán số lần lặp trong vòng lặp for
for (int i = 0; i < (1 << 10); i++) {
    // Thực hiện các thao tác trên bit
}
Không sử dụng đệ quy: Tránh sử dụng đệ quy trong các ứng dụng nhúng vì nó có thể dẫn đến việc sử dụng bộ nhớ không cần thiết. Thay vào đó, nên sử dụng vòng lặp hoặc các giải pháp khác để thực hiện các chức năng tương tự.

    Ví dụ, nếu bạn muốn tính giai thừa của một số, việc sử dụng đệ quy để tính toán sẽ dẫn đến việc cấp phát thêm bộ nhớ cho mỗi lần đệ quy. Thay vào đó, bạn có thể sử dụng một vòng lặp để tính toán giai thừa mà không cần sử dụng đệ quy.

int factorial(int n) {
   int result = 1;
   for (int i = 1; i <= n; ++i) {
      result *= i;
   }
   return result;
}
    Trong ví dụ này, chúng ta sử dụng một vòng lặp for để tính toán giai thừa của một số n. Bằng cách sử dụng vòng lặp thay vì đệ quy, chúng ta tránh việc sử dụng bộ nhớ không cần thiết và tăng hiệu suất của ứng dụng.

Quy tắc về xử lý thời gian: Không sử dụng các hàm xử lý thời gian như delay(), usleep() trong code nhúng. Thay vào đó, nên sử dụng các phương pháp hỗ trợ bởi phần cứng hoặc thư viện để đạt được các chức năng tương tự.

    Ví dụ sau đây là một chương trình đơn giản trên Arduino sử dụng hàm delay():

void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn on the LED
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn off the LED
  delay(1000);                       // wait for a second
}
    Trong ví dụ này, chương trình sử dụng hàm delay() để tạo ra một đèn LED nhấp nháy mỗi giây. Tuy nhiên, việc sử dụng hàm delay() trong code nhúng không được khuyến khích vì nó có thể làm gián đoạn các chức năng khác của hệ thống.

    Thay vào đó, bạn có thể sử dụng thư viện TimerOne của Arduino để thực hiện chức năng tương tự mà không cần sử dụng hàm delay(). Dưới đây là một ví dụ tương tự với việc sử dụng TimerOne:

#include <TimerOne.h>
int ledState = LOW;
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
  Timer1.initialize(1000000); // initialize timer to 1 second
  Timer1.attachInterrupt(timerISR); // attach interrupt service routine
}
void loop() {
  // do other things here
}
void timerISR() {
  if (ledState == LOW) {
    ledState = HIGH;
  } else {
    ledState = LOW;
  }
  digitalWrite(LED_BUILTIN, ledState);
}
    Trong ví dụ này, chúng ta sử dụng thư viện TimerOne để tạo một ngắt thời gian (interrupt) sau mỗi giây. Khi ngắt thời gian được kích hoạt, hàm timerISR() được gọi để thay đổi trạng thái của đèn LED. Bằng cách sử dụng ngắt thời gian, chúng ta có thể thực hiện chức năng nhấp nháy đèn LED mà không làm gián đoạn các chức năng khác của hệ thống.

Quy tắc về sử dụng con trỏ: Nên sử dụng con trỏ một cách cẩn thận để tránh các lỗi như tràn bộ đệm hoặc lỗi không xác định. Hạn chế sử dụng các kiểu con trỏ phức tạp và nên sử dụng các kiểu dữ liệu an toàn hơn như mảng tĩnh.
    Ví dụ:
    Trong đoạn code sau, một con trỏ được sử dụng để truy cập một mảng các số nguyên. Tuy nhiên, không có kiểm tra độ dài của mảng, do đó, nếu độ dài của mảng nhỏ hơn số lượng các phần tử được truy cập, sẽ xảy ra lỗi tràn bộ đệm:

int* myArray = new int[5];
for (int i = 0; i < 10; i++) {
  myArray[i] = i;
}
delete[] myArray;
    Để tránh lỗi tràn bộ đệm trong ví dụ này, có thể sử dụng mảng tĩnh thay vì sử dụng con trỏ:

int myArray[5];
for (int i = 0; i < 5; i++) {
  myArray[i] = i;
}
    Với việc sử dụng mảng tĩnh, độ dài của mảng được xác định trước và không thể thay đổi, do đó tránh được lỗi tràn bộ đệm.

Quy tắc về sử dụng vòng lặp: Nên sử dụng vòng lặp for thay vì while hoặc do-while nếu có thể, vì vòng lặp for có thể được tối ưu hơn và dễ đọc hơn.
    Ví dụ:
    Giả sử chúng ta muốn tính tổng của một mảng số nguyên. Ta có thể sử dụng vòng lặp for để làm điều đó như sau:

int arr[] = {1, 2, 3, 4, 5};
int sum = 0;
for (int i = 0; i < 5; i++) {
    sum += arr[i];
}
    Trong ví dụ trên, ta sử dụng vòng lặp for để duyệt qua các phần tử trong mảng và tính tổng của chúng. Vòng lặp for có thể dễ dàng được tối ưu hơn bởi trình biên dịch và nó cũng giúp cho code dễ đọc hơn so với sử dụng while hoặc do-while.

Quy tắc về sử dụng biến toàn cục: Hạn chế sử dụng biến toàn cục trong code nhúng vì nó có thể gây ra các lỗi không xác định và khó để theo dõi. Thay vào đó, nên sử dụng các biến cục bộ hoặc truyền các giá trị vào hàm.
    Ví dụ:
int count = 0; // Biến toàn cục
void loop() {
  count++;
  Serial.println(count);
}
    Trong ví dụ này, biến count được khai báo là biến toàn cục, có thể được truy cập từ bất kỳ hàm nào trong chương trình. Tuy nhiên, sử dụng biến toàn cục như vậy có thể gây ra các lỗi không xác định và khó để theo dõi, đặc biệt là trong các chương trình lớn hơn.

    Thay vào đó, chúng ta nên sử dụng các biến cục bộ hoặc truyền các giá trị vào hàm để hạn chế sử dụng biến toàn cục. Ví dụ, ta có thể sửa đổi ví dụ trên để sử dụng biến cục bộ như sau:

void loop() {
  int count = 0; // Biến cục bộ
  count++;
  Serial.println(count);
}
    Hoặc chúng ta có thể truyền giá trị vào hàm để thay thế cho biến toàn cục, ví dụ như sau:

void loop() {
  static int count = 0; // Biến tĩnh
  count = incrementCount(count);
  Serial.println(count);
}
int incrementCount(int count) {
  count++;
  return count;
}
    Trong ví dụ này, ta sử dụng biến tĩnh và truyền giá trị count vào hàm incrementCount(). Hàm này sẽ tăng giá trị count lên một đơn vị và trả về giá trị mới. Hàm loop() sau đó lấy giá trị trả về và in ra màn hình. Việc sử dụng biến tĩnh giúp ta lưu trữ giá trị của biến count giữa các lần gọi hàm, giúp chương trình hoạt động đúng như mong đợi.

7. Quy tắc về biểu thức và toán tử

Tránh sử dụng các biểu thức phức tạp: Nên tách các biểu thức phức tạp thành các biểu thức đơn giản hơn để dễ đọc và hiểu hơn.

    Ví dụ:

//Thay vì viết
if ((x > 10 && y < 5) || (x <= 10 && y >= 5)) {
    // do something
}
//Nên viết lại thành
bool isXGreaterThanTen = (x > 10);
bool isYLessThanFive = (y < 5);
bool isXLessThanOrEqualToTen = (x <= 10);
bool isYGreaterThanOrEqualToFive = (y >= 5);
if ((isXGreaterThanTen && isYLessThanFive) || (isXLessThanOrEqualToTen && isYGreaterThanOrEqualToFive)) {
    // do something
}
    Viết lại biểu thức này giúp cho code dễ đọc và hiểu hơn, cũng như tránh các lỗi có thể xảy ra khi đánh giá biểu thức phức tạp.

Hạn chế sử dụng toán tử động (dynamic operator): Các toán tử động như truy cập con trỏ và chuyển đổi kiểu dữ liệu có thể gây ra các lỗi không xác định và khó theo dõi.
    Ví dụ:
int *ptr = NULL;
int a = 10;
ptr = &a; // gán con trỏ ptr trỏ đến địa chỉ của biến a
*ptr = 20; // thay đổi giá trị của biến a thông qua con trỏ ptr
float *fptr = NULL;
fptr = (float *)&a; // ép kiểu con trỏ fptr sang kiểu float và trỏ đến địa chỉ của biến a
*fptr = 3.14; // thay đổi giá trị của biến a thông qua con trỏ fptr, điều này có thể gây ra lỗi không xác định
    Trong ví dụ trên, toán tử động được sử dụng để truy cập con trỏ và chuyển đổi kiểu dữ liệu. Việc sử dụng toán tử động này có thể dẫn đến các lỗi không xác định và khó theo dõi, đặc biệt là khi sử dụng với các kiểu dữ liệu không phù hợp. Do đó, nên hạn chế sử dụng toán tử động trong code của mình.

Luôn sử dụng các toán tử an toàn (safe operators): Sử dụng các toán tử an toàn như &&, || và ! thay vì & và | để tránh các lỗi không xác định và đảm bảo rằng các biểu thức được đánh giá một cách đúng đắn.
    Ví dụ:

int a = 5, b = 10, c = 0;
// Sử dụng toán tử && an toàn để kiểm tra giá trị của a và b
if (a > 0 && b < 20) {
  // Nếu a lớn hơn 0 và b nhỏ hơn 20, thì thực hiện phép tính
  c = a + b;
}
    Trong ví dụ này, ta sử dụng toán tử && an toàn để kiểm tra giá trị của biến a và b. Nếu cả hai biến này thỏa mãn điều kiện được đưa ra, thì phép tính c = a + b sẽ được thực hiện. Nếu không, phép tính này sẽ được bỏ qua. Sử dụng toán tử && an toàn này giúp đảm bảo rằng các biểu thức được đánh giá một cách đúng đắn và tránh các lỗi không xác định.

 
Sử dụng toán tử cộng (+) để thay thế cho toán tử nối chuỗi (+): Toán tử nối chuỗi (+) có thể dẫn đến các lỗi không xác định khi sử dụng với các kiểu dữ liệu không phải là chuỗi. cho ví dụ
    Ví dụ:

int x = 5;
char str[10] = "hello";
char new_str[20];
// sử dụng toán tử nối chuỗi (+)
sprintf(new_str, "%d" + str); // lỗi! không thể nối chuỗi số và chuỗi kí tự
// sử dụng toán tử cộng (+) thay thế
sprintf(new_str, "%d%s", x, str); // đúng đắn, nối chuỗi số và chuỗi kí tự bằng toán tử cộng
    Trong ví dụ này, khi sử dụng toán tử nối chuỗi (+), ta không thể nối chuỗi số và chuỗi kí tự với nhau, dẫn đến lỗi không xác định. Thay vào đó, ta có thể sử dụng toán tử cộng (+) để nối chuỗi số và chuỗi kí tự với nhau một cách đúng đắn.

Hạn chế sử dụng các toán tử bit (bitwise operator): Các toán tử bit có thể dẫn đến các lỗi không xác định khi sử dụng với các kiểu dữ liệu không phải là số nguyên.
    Ví dụ:
float a = 3.5;
float b = 2.0;
float c = a | b; // Lỗi biên dịch: toán tử bit không áp dụng cho kiểu dữ liệu float
    Trong ví dụ này, ta có hai biến kiểu dữ liệu float là a và b. Khi sử dụng toán tử bit | để gán giá trị của biểu thức a | b cho biến c, ta sẽ nhận được một lỗi biên dịch vì toán tử bit không áp dụng cho kiểu dữ liệu float. Do đó, ta cần hạn chế sử dụng toán tử bit trên các kiểu dữ liệu không phải là số nguyên.

Sử dụng các biểu thức phù hợp với kiểu dữ liệu của biến: Sử dụng các biểu thức phù hợp với kiểu dữ liệu của biến để đảm bảo rằng các phép tính được đánh giá một cách đúng đắn và an toàn.
    Ví dụ:
    Nếu có một biến kiểu số nguyên int và một biến kiểu số thực float, khi thực hiện phép toán trên hai biến này cần đảm bảo rằng toán tử được sử dụng phù hợp với kiểu dữ liệu tương ứng của từng biến. Ví dụ, nếu bạn muốn tính tổng của hai biến này, bạn cần sử dụng toán tử cộng (+) với hai toán hạng cùng kiểu số (hoặc chuyển đổi kiểu dữ liệu phù hợp trước khi thực hiện phép tính).
int a = 5;
float b = 2.5;
float sum = a + b; // lỗi biên dịch, cần chuyển đổi kiểu dữ liệu
float sum = a + (float)b; // đúng
    Trong ví dụ này, nếu không chuyển đổi kiểu dữ liệu của biến a sang kiểu float trước khi thực hiện phép tính, chương trình sẽ không biên dịch được vì hai toán hạng không cùng kiểu dữ liệu.

Sử dụng các toán tử so sánh an toàn: Sử dụng các toán tử so sánh an toàn như ==, !=, <, >, <= và >= để tránh các lỗi không xác định và đảm bảo rằng các biểu thức được đánh giá một cách đúng đắn.
    Ví dụ:

#include <stdio.h>
int main() {
   int a = 10, b = 5, c = 10;
   // sử dụng toán tử so sánh an toàn ==
   if (a == b) {
      printf("a bằng b\n");
   } else {
      printf("a không bằng b\n");
   }
   if (a == c) {
      printf("a bằng c\n");
   } else {
      printf("a không bằng c\n");
   }
   // sử dụng toán tử so sánh an toàn <
   if (b < a) {
      printf("b nhỏ hơn a\n");
   } else {
      printf("b không nhỏ hơn a\n");
   }
   // sử dụng toán tử so sánh an toàn <=
   if (a <= c) {
      printf("a nhỏ hơn hoặc bằng c\n");
   } else {
      printf("a không nhỏ hơn hoặc bằng c\n");
   }
   return 0;
}
    Kết quả của chương trình trên sẽ là:

a không bằng b
a bằng c
b nhỏ hơn a
a nhỏ hơn hoặc bằng c
    Chương trình trên sử dụng các toán tử so sánh an toàn để so sánh giá trị của các biến kiểu số nguyên và đảm bảo rằng các biểu thức được đánh giá một cách đúng đắn.

8. Quy tắc về hàm và tham số

Tên hàm và tham số:
    – Tên hàm và tham số nên được đặt sao cho dễ hiểu và mô tả được chức năng của chúng.
    – Tên hàm nên bắt đầu bằng một động từ hoặc chữ viết tắt mô tả chức năng của hàm.
    – Tên tham số nên được đặt sao cho mô tả được dữ liệu mà tham số đại diện.
Tên hàm: Bắt đầu bằng một động từ mô tả chức năng của hàm, ví dụ như calculate, initialize, validate, set, get, process,…
Tên tham số: Nên được đặt sao cho mô tả được dữ liệu mà tham số đại diện, ví dụ như input, output, value, pointer, length, index,…
Nên tránh viết tắt và các ký tự đặc biệt.

    Ví dụ:

// Hàm tính giá trị tuyệt đối của số nguyên
int calculateAbsoluteValue(int input);
// Hàm đặt giá trị cho biến
void setVariableValue(int *pointer, int value);
// Hàm xử lý chuỗi
void processString(char *inputString, int length);
// Hàm lấy giá trị từ mảng
int getValueFromArray(int *array, int index);
Định dạng hàm:
    – Hàm nên được định dạng sao cho dễ đọc và dễ hiểu.
    – Hàm nên được phân chia thành các phần rõ ràng như đầu vào, xử lý và đầu ra.
    – Hàm nên được viết theo một chuẩn nhất định để dễ đọc và hiểu.
    Ví dụ về việc định dạng hàm cho một thuộc tính trong một struct như sau:

/**
 * @brief Structure containing the properties of a car
 */
typedef struct {
    uint8_t speed;  /**< Speed of the car in km/h */
    uint8_t fuel_level;  /**< Fuel level of the car in percent */
} car_properties_t;
/**
 * @brief Function to update the speed of a car
 *
 * @param car Pointer to the car properties struct
 * @param new_speed The new speed of the car in km/h
 */
void update_car_speed(car_properties_t *car, uint8_t new_speed)
{
    car->speed = new_speed;
}
    Trong ví dụ này, hàm update_car_speed được định dạng rõ ràng với đầu vào là car và new_speed, và không có giá trị trả về. Hàm được chia thành các phần rõ ràng như đầu vào (car và new_speed), xử lý (cập nhật giá trị của thuộc tính speed trong car) và không có đầu ra.

    Ngoài ra, các comment được sử dụng để giải thích chức năng của hàm và các thuộc tính của struct, giúp cho việc đọc code dễ hiểu và dễ bảo trì hơn.

Các quy tắc về tham số: Tham số đầu vào nên được khai báo là const để bảo vệ chúng khỏi việc thay đổi bất hợp lý.
    Ví dụ:

void print_array(const int *arr, int size) {
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
}
    Trong ví dụ này, tham số đầu vào arr được khai báo là const int *, cho phép hàm sử dụng giá trị của mảng arr nhưng không cho phép thay đổi giá trị của mảng này.

Tham số nên được truyền theo giá trị nếu không cần thiết phải thay đổi giá trị đó.

    Ví dụ:

int sum(int a, int b) {
    return a + b;
}
    Trong ví dụ này, tham số a và b được truyền theo giá trị, vì hàm sum không cần phải thay đổi giá trị của a và b.

Tham số nên được truyền theo con trỏ nếu cần phải thay đổi giá trị đó.

    Ví dụ;

void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
    Trong ví dụ này, tham số a và b được truyền theo con trỏ, cho phép hàm swap thay đổi giá trị của a và b bằng cách sử dụng con trỏ.

Các quy tắc về giá trị trả về của hàm:
    – Hàm nên trả về một giá trị duy nhất để tránh lỗi không xác định.

    – Giá trị trả về của hàm nên được xác định trước khi thực hiện hàm và được đưa ra trong tài liệu hướng dẫn sử dụng của hàm.

    – Giá trị trả về của hàm nên được xử lý sao cho phù hợp với mục đích của hàm.

    Ví dụ:

/**
 * @brief Tính tổng các phần tử trong một mảng.
 * 
 * @param arr Mảng đầu vào.
 * @param size Kích thước của mảng.
 * @return Tổng các phần tử trong mảng.
 */
int sumArray(const int arr[], int size) {
    int sum = 0;
    for(int i = 0; i < size; i++) {
        sum += arr[i];
    }
    return sum;
}
    Trong ví dụ này, hàm sumArray trả về một giá trị nguyên duy nhất – tổng các phần tử trong mảng đầu vào. Giá trị trả về đã được xác định trước khi thực hiện hàm và được đưa ra trong tài liệu hướng dẫn sử dụng của hàm. Ngoài ra, giá trị trả về đã được xử lý sao cho phù hợp với mục đích của hàm – tính tổng các phần tử trong mảng.

Các quy tắc về việc gọi hàm:
    – Gọi hàm với đúng tên và đúng kiểu trả về của hàm

    – Gọi hàm với đúng số lượng tham số và kiểu dữ liệu của chúng

    – Gọi hàm với các tham số hợp lệ để tránh lỗi không xác định

    – Gọi hàm với đúng thứ tự của các tham số

    Ví dụ:

// Hàm tính diện tích hình chữ nhật
float calculateRectangleArea(float length, float width) {
    return length * width;
}
int main() {
    float length = 4.0;
    float width = 5.0;
    // Gọi hàm tính diện tích hình chữ nhật với các tham số đúng kiểu và đúng thứ tự
    float area = calculateRectangleArea(length, width);
    return 0;
}
    Trong ví dụ trên, hàm calculateRectangleArea được gọi với đúng kiểu và đúng thứ tự của các tham số, và sử dụng các biến hợp lệ là length và width để tính toán diện tích của hình chữ nhật.

9. Quy tắc về cấu trúc và liên kết

– Tập tin mã nguồn nên được phân chia thành các tập tin nhỏ hơn để dễ dàng quản lý và tái sử dụng mã.

– Tên các tập tin và biến nên được đặt sao cho dễ hiểu và mô tả được chức năng của chúng.

– Các biến và hằng nên được khai báo ở đầu tập tin và được sắp xếp theo thứ tự chữ cái.

– Các hằng số nên được định nghĩa bằng các macro và được đặt tên theo dạng chữ hoa và các từ cách nhau bởi dấu gạch dưới.

– Các hàm nên được sắp xếp theo thứ tự chức năng và tên hàm nên được đặt sao cho mô tả được chức năng của hàm.

– Các hàm nên được định nghĩa trước khi sử dụng và các hàm nên được khai báo ở đầu tập tin.

– Tên tham số của các hàm nên được đặt sao cho mô tả được dữ liệu mà tham số đại diện.

– Các lệnh nên được định dạng sao cho dễ đọc và dễ hiểu.

– Các khối lệnh nên được đặt trong cặp dấu ngoặc nhọn và được thụt đầu dòng sao cho dễ đọc và hiểu.

– Các biến nên được khai báo ở phạm vi nhỏ nhất có thể để tránh lỗi không xác định.

    Ví dụ:

// Định nghĩa macro
#define MAX_SIZE 100
// Khai báo biến và hằng
int i, j;
const float PI = 3.14;
// Định nghĩa hàm
int add(int a, int b) {
  return a + b;
}
// Sử dụng hàm
int result = add(3, 4);
// Định dạng các lệnh và khối lệnh
if (result == 7) {
  printf("The result is correct!\n");
} else {
  printf("The result is incorrect!\n");
}
10. Quy tắc về xử lý chuỗi

– Sử dụng hằng số để lưu độ dài tối đa của chuỗi.

– Sử dụng các hàm chuẩn như strncpy() hoặc memcpy() để sao chép chuỗi.

– Kiểm tra kích thước đầu vào của chuỗi để tránh các lỗi tràn bộ đệm.

– Sử dụng các hàm chuẩn như strcmp() hoặc strncmp() để so sánh chuỗi.

– Sử dụng các hàm chuẩn như strcat() hoặc strncat() để nối chuỗi.

– Kiểm tra giá trị trả về của các hàm xử lý chuỗi để xử lý các lỗi.

    Ví dụ:

#include <stdio.h>
#include <string.h>
#define MAX_LENGTH 100
void copyString(char *dest, const char *src)
{
    size_t length = strlen(src);
    if (length >= MAX_LENGTH)
    {
        printf("Error: source string is too long\n");
        return;
    }
    strncpy(dest, src, length);
    dest[length] = '\0';
}
int main()
{
    char str1[MAX_LENGTH] = "Hello";
    char str2[MAX_LENGTH] = "World";
    char str3[MAX_LENGTH];
    copyString(str3, str1);
    printf("str3: %s\n", str3);
    strcat(str1, " ");
    strncat(str1, str2, MAX_LENGTH - strlen(str1) - 1);
    printf("str1: %s\n", str1);
    if (strncmp(str1, "Hello World", MAX_LENGTH) == 0)
    {
        printf("The strings match!\n");
    }
    else
    {
        printf("The strings do not match.\n");
    }
    return 0;
}
    Trong ví dụ trên, hàm copyString() được sử dụng để sao chép chuỗi từ src sang dest. Hằng số MAX_LENGTH được sử dụng để giới hạn độ dài của chuỗi và tránh lỗi tràn bộ đệm. Hàm strncat() được sử dụng để nối chuỗi str2 vào str1 với số lượng ký tự tối đa được tính toán để tránh lỗi tràn bộ đệm. Hàm strncmp() được sử dụng để so sánh hai chuỗi. Giá trị trả về của các hàm xử lý chuỗi được kiểm tra để xử lý các lỗi.

11. Quy tắc về xử lý số học

– Tránh sử dụng toán tử chia (/) với số nguyên: Nếu một biểu thức chứa toán tử chia (/) với số nguyên, kết quả sẽ được chuyển đổi thành số nguyên và làm tròn về phía không gần nhất. Điều này có thể dẫn đến sai sót trong tính toán.

– Sử dụng phép chia hợp lệ cho số thực: Tránh sử dụng toán tử chia (/) với số thực, vì nó có thể dẫn đến sai số trong tính toán. Thay vào đó, sử dụng các phép chia hợp lệ cho số thực như phép chia liên tục (floating-point division) hoặc phép nhân với nghịch đảo (multiply by inverse).

– Tránh tràn số: Khi thực hiện các phép tính số học, cần kiểm tra tràn số để tránh kết quả không xác định hoặc sai sót trong tính toán.

– Sử dụng các hàm toán học chuẩn: Các hàm toán học chuẩn như sqrt(), sin(), cos(), tan() đã được kiểm tra và xác định rằng chúng hoạt động đúng với mọi trường hợp. Vì vậy, nên sử dụng các hàm này thay vì tự viết hàm toán học của riêng mình.

– Đảm bảo độ chính xác của tính toán: Khi thực hiện các tính toán phức tạp hoặc yêu cầu độ chính xác cao, cần sử dụng các thư viện toán học đáng tin cậy hoặc các thuật toán tính toán độ chính xác cao.

    Ví dụ, theo tiêu chuẩn Autosar C Coding Guidelines, nếu ta muốn tính giá trị của sin(x) với x là một số thực, ta nên sử dụng hàm sin() được cung cấp sẵn trong thư viện math.h thay vì tự viết hàm sin() của riêng mình. Nếu muốn kiểm tra độ chính xác của kết quả, ta có thể so sánh giá trị tính toán được với giá trị đã biết của sin(x) trong một số trường hợp cụ thể.






