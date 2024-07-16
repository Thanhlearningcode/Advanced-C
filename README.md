Lesson 3: POINTER
Trong ngôn ngữ lập trình C, con trỏ (pointer) là một biến chứa địa chỉ bộ nhớ của một biến khác. Việc sử dụng con trỏ giúp chúng ta thực hiện các thao tác trên bộ nhớ một cách linh hoạt hơn.
Cách khai báo:      datatype * PointerName; 	
A. Void Pointer
Là một con trỏ đặc biệt có thể trỏ tới các đối tượng thuộc bất kỳ kiểu dữ liệu nào.
Cách khai báo:      void *PointerName; 
Ex:
#include <stdio.h>
#include<stdint.h>
int main()
{
	int int_var = 63;
	char char_var = 'f';
	void* ptr = &int_var;
	printf("%p\n", ptr);
	ptr = &char_var;
	printf("%p\n", ptr);
}
 
 
B. Function Pointer
Là một biến mà giữ địa chỉ của một hàm, nó trỏ đến vùng nhớ trong bộ nhớ chứa mã máy của hàm được định nghĩa trong chương trình.
Cách khai báo:      <return_type>  (*<PointerName>)( <ParametersDataType> );
Ex:
void Tong(int a, int b)
{
	printf("Tong cua %d va %d la: %d\n", a, b, a + b);
}
void Hieu(int a, int b)
{
	printf("Hieu cua %d va %d la: %d\n", a, b, a - b);
}
void Tich(int a, int b)
{
	printf("Tich cua %d va %d la: %d\n", a, b, a * b);
}
void Thuong(int a, int b)
{	
	if(b==0){
	Printf("B phai khac 0");
	}
	Else
	printf("Thuong cua %d va %d la: %f\n", a, b, a/(double)b);
}

void TinhToan(void (*pheptoan)(int,int), int a, int b) {
	pheptoan(a, b);
}

int main()
{
	//tạo 1 mảng chứa các con trỏ hàm cho từng hàm riêng biệt
	void (*pheptoan[])(int, int) = { &Tong,&Hieu,&Tich,&Thuong };

	TinhToan(&Tong, 10, 5);
	TinhToan(&Hieu, 10, 5);
	TinhToan(&Thuong, 10, 5);
	TinhToan(&Tich, 10, 5);
	
	return 0;
}
 
C. Pointer to Constant
Định nghĩa một con trỏ không thể thay đổi giá trị tại địa chỉ mà nó trỏ đến thông qua dereference nhưng giá trị tại địa chỉ đó có thể thay đổi.
Cách khai báo:     int const *ptr_const;
		     const int *ptr_const;
Ex:
int value = 5;
int const* ptr_const = &value;
printf("value: %d\n", *ptr_const);
value = 9;
printf("value: %d\n", *ptr_const);
return 0;

D. Constant Pointer
Định nghĩa một con trỏ mà giá trị nó trỏ đến không thể thay đổi. 
Cách khai báo:     int *const const_ptr = &value;
Ex:
int value = 5;
int* const const_ptr = &value;
printf("value: %d\n", *const_ptr);
*const_ptr = 7;
printf("value: %d\n", *const_ptr);
return 0;
 
E. Pointer to Pointer
Là kiểu dữ liệu trong ngôn ngữ lập trình cho phép lưu trữ địa chỉ của một con trỏ	
Cách khai báo: int *ptr = &test;
                             int **ptp = &ptr;
Ex:
int value = 5;
int* ptr = &value; // khai báo biến con trỏ chứa địa chỉ của value
int** ptp = &ptr; //con trỏ chứa địa chỉ của con trỏ ptr
printf("Dia chi cua value: %p\n",ptr);
printf("Gia cua value: %d\n", *ptr);
printf("Dia chi cua ptr: %p\n", ptp);
printf("Gia cua ptr: %p\n", *ptp);
return 0;
 
F. NULL Pointer
Là một con trỏ không trỏ đến bất kỳ đối tượng hoặc vùng nhớ cụ thể nào. Sử dụng null pointer thường hữu ích để kiểm tra xem một con trỏ đã được khởi tạo và có trỏ đến một vùng nhớ hợp lệ chưa.
Ex:
int* ptr = NULL; 
if (ptr == NULL) {
	printf("Pointer is NULL\n");
}
else {
	printf("Pointer is not NULL\n");
}

