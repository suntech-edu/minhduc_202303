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