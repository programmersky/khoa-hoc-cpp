---
title : Cấu trúc rẽ nhánh khác (if...else if ..., cấu trúc if lồng nhau)
---

>Chúng ta sẽ cùng sử dụng kiến thức của bài if else và toán tử logic để cùng tìm hiểu bài này.
>Hi vọng các bạn nắm chắc kiến thức bài trước. Để không khỏi bỡ ngỡ tại bài này.

Ví dụ: Nhập vào một số nguyên. Kiểm tra xem số đó có là số dương hay không ? Nếu có thì in ra màn hình thông báo là số dương. Nếu không thì in ra màn hình là số âm.

Các bạn tham khảo đoạn code sau : 
  
    	
    	#include<iostream>
    	using namespace std;
    	int main()
    	{
    	int n;
    	
    	cout << " Nhap vao so nguyen "<< endl;
    	cin >> n;
    	
    		if( n > 0)
    			{
    				cout << n << " la so duong " << endl;
    			}
    		else 
    			{
    				cout << n << " la so am" << endl;
    			}
    return 0;	
	}
    	
**Input 1**

	n=10;

**Output 1**
  	
	10 la so duong


**Input 2**

	n=-10;

**Output 2**
  	
	-10 la so am

**Input 3**

	n=0;

**Output 3**
  	
	0 la so am

###Có điều gì đó không ổn ở Output số 3 rồi.

Vì vậy, bài toán chưa thực sự hoạt động tốt.
Chúng ta sẽ sử dụng cấu trúc if esle if lồng nhau để giải quyết vấn đề này.



	 #include<iostream>
    	using namespace std;
    	int main()
    	{
    	int n;
    	
    	cout << " Nhap vao so nguyen "<< endl;
    	cin >> n;
    	
    		if( n > 0)
    			{
    				cout << n << " la so duong " << endl;
    			}
    		else
    			{
					if( n < 0)
						{
    							cout << n << " la so am" << endl;
    						}
					else	
						{
							cout << n << " la so 0" << endl;	
						}
				}
    return 0;	
	}


**Input 1**

	n=10;

**Output 1**
  	
	10 la so duong


**Input 2**

	n=-10;

**Output 2**
  	
	-10 la so am

**Input 3**

	n=0;

**Output 3**
	
	0 la so 0


----------

Chúng ta có thể diễn giải đoạn code trên như sau : 

**Nếu** *n > 0*  **thì** *in ra* màn hình  **n là số dương**

**Ngược lại** *n không lớn hơn 0*, **thì** chỉ có 2 trường hợp là *nhỏ hơn 0* hoặc *bằng 0*.

**Tiếp tục** kiểm tra **nếu** *n<0* **thì** *in ra* màn hình **n là số âm**. 

**Nếu** *n không nhỏ hơn không* **thì** lúc này chắc chắn **n bằng 0** và *in ra* màn hình **n là số 0**
 

>Các bạn có thể áp dụng if else if một cách linh hoạt tùy vào từng trường hợp.

**Lưu ý**: Trong khối lệnh sau if hoặc else chúng ta có thể gọi thêm các cấu trúc if else khác. Nhưng phải để ý tới điều kiện của biểu thức để tránh có lỗi không mong muốn.


----------

Áp dụng : 
 Các bạn đã có thể làm một trò kinh điển đơn giản sử dụng với việc sử dụng if else if.
### Búa Giấy Kéo...
Xây dụng một ứng dụng console. Cho phép nhập vào lựa chọn 

**1** ứng với **Búa**
 
**2** ứng với **Giấy**

**3** ứng với **Kéo**

Kiểm tra việc nhập và in ra màn hình xem người dùng vừa lựa chọn Búa , Giấy hay Kéo.

> Nâng cấp. Cho 2 người dùng lần lượt chọn. Sau đó kiểm tra xem sự lựa chọn của người dùng nào thắng. Và in ra màn hình người thắng cuộc

> Búa thắng Kéo.
> 
> Kéo thắng Giấy.
> 
> Giấy Thắng Búa.


----------
P/s: **Hẹn gặp lại các bạn trong bài học tiếp theo trong khóa học lập trình C++ hướng thực hành.**


Mọi ý kiến đóng góp hoặc thắc mắc có thể đặt câu hỏi trực tiếp tại diễn đàn 

[www.daynhauhoc.com](www.daynhauhoc.com "DayNhauHoc")
