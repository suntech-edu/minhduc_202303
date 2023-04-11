01. Phân loại thẻ HTML
    - block: chiếm 100% chiều rộng của trình duyệt
        ex: <div></div>
    - inline: chiều rộng thẻ đúng bằng chiều rộng của nội dung mà nó chứa
        ex: <span></span>
    - none: không hiển thị lên trình duyệt
        ex: <meta></meta>

02. Tại sao phải sử dụng css:
    - giảm dung lượng cho file
    - tiết kiệm thời gian
    - làm giao diện trang đẹp hơn

03. Khai báo trong css
    có 3 cách khai báo:
        - khai báo nội tuyến(internal)
            ex: <style>
                    code css
                </style>
        - khai báo ngoại tuyến(external)
            ex: nhúng file css từ bên ngoài vào thông qua thẻ <link>
                <link rel="stylesheet" href="style.css">
        - khai báo trực tiếp tại thẻ(inline)
             ex: sử dụng thuộc tính style ngay trong thẻ mở của thẻ

04. Độ ưu tiên trong css

    - Nội tuyến
    - Ngoại tuyến
    - Inline
        ==> thuộc tính được khai báo sau cùng được ưu tiên
    - độ ưu tiên của class & id & tên thẻ
        ==> độ ưu tiên của id > class > tên thẻ
    - Từ !important
        ==> có độ ưu tiên cao nhất bất kể nó đứng ở đâu

05. Cú pháp định nghĩa css cho một thẻ

    selector {
    	css-attribute-name-1: value1;
    	css-attribute-name-2: value2;
    	css-attribute-name-3: value3;
    	...
    	css-attribute-name-n: valuen;
    }

21. Sprite css

    thay vì load từng ảnh nhỏ ta đưa nó vào 1 ảnh lớn và load lên trang 1 lần duy nhất, khi nào dùng đến sẽ lấy ra bằng thuộc tính "background-position"
06. Các loại selector trong css

*Các loại selector thường dùng
    - selector theo tên thẻ
        ex: h1{}
    - selector theo tên class
        ex: .name{}
    - selector theo tên id
        ex: #name{}
    - selector theo attribute của thẻ html
        ex: input [type="text"]{}
    - * chọn tất cả các thẻ
        ex: *{}
    - Nhóm các selector bằng dấu ","
        ex: h1, h2, h3{}

07. Select theo thứ tự của thẻ
- :fist-of-type  --> lấy ra thẻ đầu tiên trong danh sách
    ex: p:fist-of-type{}

- :last-of-type  --> lấy ra thẻ cuối cùng trong danh sách
    ex: p:last-of-type{}

- :nth-of-type(n)  --> lấy ra thẻ thứ n trong danh sách
    ex: p:nth-of-type(n){}


08. Selector theo hành động của người dùng:

    - :hover{
        'code css'
        }
    --> chỉ con trỏ chuột đến nội dung. 

    - :active{
        'code css'
    }
    --> click chuột vào nội dung. 

    - :focus{
        'code css'
    }
    --> click chọn nội dung(thường dùng cho input). 

    - :checked{
        'code css'
    }
    --> click chọn 1 check box trong input type="checkbox"

    09. Css Pseudo element
        ::first-letter{
                "css"
            }
        --> Chữ cái đầu tiên của nội dung

        ::first-line{
                "css"
            }
        --> Dòng đầu tiên của nội dung

        ::before{
                content:"nội dung muốn thêm vào trước nội dung sẵn có";
            }

        ::after{
                content:"nội dung muốn thêm vào sau nội dung sẵn có";
            }

10. Parent selector
    Dùng trong trường hợp có nhiều thẻ, class lồng nhau, parenr selector có tác dụng lấy ra phần tử có cha trực tiếp là class được chọn.
    selectorParent > selectChirend

    ex:     
        .root > p{
            css
        }

11. Phân biệt "class" và "id"

    - Class: Được phép định nghĩa nhiều lần trên cùng 1 trang,
            Dùng để quy định CSS giống nhau cho một nhóm thẻ HTML có chung các đặc điểm
    
    - ID: Tồn tại duy nhất 1 id trên 1 trang, không được phép định nghĩa 2 lần

12. Các đơn vị đo lường trong css

    Được dùng để quy định kích thước, chiều rộng, chiều cao, cỡ chữ hay nội dung của thẻ html...

    * Đơn vị tuyệt đối: cố định, không thay đổi, không phụ thuộc vào màn hình hay thẻ chứa nó
        - px
        - pt
        - cm
        - mm
        - in
    * Đơn vị tương đối: sẽ biến đổi khi chạy trên các thiết bị có màn hình khác nhau và phụ thuộc vào thẻ chứa nó
        - %
        - em
        - rem

16. Phạm vi sử dụng của biến trong css

    - biến khia báo trong :root có thể dùng được ở mọi nơi(biến toàn cục).
    - biến khai báo trong selector thì chỉ có tác dụng với các thành phần con của selector đó(biến cục bộ)

17. Ghi đè một biến trong css

    Việc ghi đè hoàn toàn không ảnh hưởng gì đến giá trị của biến ban đầu, nó chỉ ảnh hưởng trong phạm vi của selector chứa biến đã được ghi đè.

18. Thuộc tính của text:
	color: màu của text
		ex: color: #000; (mã màu)
	
	text-align: căn chỉnh nội dung theo chiều ngang
		ex: text-align: left; (vị trí)

	text-decoration: trang trí thêm cho text
		ex: text-decoration: overline; (thêm dòng kẻ phía trên cho text)
        
	text-transform: quy định kiểu chữ viết hoa hay viết thường
		ex: text-transform: uppercase; (chữ viết hoa)
        
