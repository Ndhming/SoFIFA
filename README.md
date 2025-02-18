
# Xây dựng mô hình hồi quy tuyến tính để dự đoán giá trị cầu thủ ⚽⚽

## Giới thiệu
Đây là dự án đầu tiên của tôi trên con đường trở thành một Data Analyst. Dự án này sẽ bao gồm đầy đủ các bước của một chu trình OSEMN (Obatain - Scrub - Explore - Model - iNterpret) một data project life cycle cơ bản. Và tất cả mọi thứ đều cơ bản thôi.

Từng stage một của dự án sẽ được tôi gắn vào trong file ggdocs, bao gồm tất cả những thông tin mà tôi nghĩ là nó sẽ đủ để hiểu được nội dung của từng bước, cách setup, các lỗi khó chịu đã gặp phải, những logic cơ bản nằm trong từng bước đó, và kết quả tôi rút ra được sau quá trình học hỏi.

Đây sẽ giống một chiếc nhật ký hơn là một báo cáo về dự án cá nhân nên mong mọi người không quá khắt khe với nó.

## Đôi nét về dự án
Dự án này lấy cảm hứng từ một project cá nhân khác tôi tìm được trên github ['đây nhé'](https://medium.com/@yulasozen/predicting-football-players-market-value-using-machine-learning-b28be298e91e) và kiến thức bổ ích từ môn kinh tế lượng trên trường.

Dự án này nhằm áp dụng các mô hình học máy để dự đoán giá trị thị trường của các cầu thủ bóng đá. Dữ liệu sẽ được thu thập từ trang web [SoFIFA](https://sofifa.com/players), bao gồm thông tin cá nhân, chỉ số cá nhân và các yếu tố ảnh hưởng khác. Sau đó, các mô hình học máy sẽ được huấn luyện để phân tích và dự đoán giá trị của cầu thủ dựa trên dữ liệu này.

Đây là một bài báo rất đầy đủ giới thiệu chi tiết từng bước một về quá trình dựng nên project này. Tôi đã học hỏi nhiều và cũng có những cải tiến của riêng mình (cụ thể ra sao tôi sẽ liệt kê ở từng bước). 



Có thể chỉ là quan điểm chủ quan của cá nhân, nhưng tôi cho rằng tập dữ liệu này không phù hợp để xây dựng mô hình hồi quy tuyến tính với phương pháp ước lượng OLS. Lí do sẽ được tôi giải thích chi tiết trong docs. 

Còn về tại sao không chạy mô hình khác để tiếp tục kiểm chứng hồi quy thì là do tôi cảm thấy mình chưa có đủ kiến thức về Machine Learning và hiện tại nó cũng chưa có tính thực tế với một intern DA hiện tại.

## Các bước của dự án

- [Obtain](https://docs.google.com/document/d/1jsjYQh4Pus-UZtfQ5M7ArwIBl2BMt1OPhGVv2c0gU98/edit?usp=sharing) - Thu thập dữ liệu bằng cách crawl data từ web (lần đầu tiên tôi thực sự học một cái gì đó nghiêm túc và cảm thấy thỏa mãn khi code chạy được)
- [Scrub](https://docs.google.com/document/d/1v6Iup1SmxpUadyzGJ8nPs8rAvjBy9RTuZuxJ03hwKGE/edit?usp=sharing) - Làm sạch dữ liệu (dữ liệu về cơ bản khá clean rồi nên chỉ cần xử lý nhẹ nhàng)
- [Explore](https://docs.google.com/document/d/1_o8dSmezSsy9nMBNARIhw64BOPkQWXW3ZCDqqdR3tE8/edit?usp=sharing) - Khám phá dữ liệu (cũng chỉ dừng lại ở mức Descriptive statistics nhẹ nhàng thôi)
- [Model](https://docs.google.com/document/d/1X2pkwRl1E3ntQYkYgPY6xa20XM5nKK1CauXnvKauHRI/edit?usp=sharing) - Xây dựng mô hình (khá là mất sức để tìm cách pass cả 6 kiểm định một lúc @@)
- [iNterpret] - Không có gì để nói, những gì muốn nói đều ở bên trên hết rồi... 

Trong mỗi link ggdocs sẽ có thể có nhiều hơn 1 thẻ (nó nằm ở bên tay trái màn hình) nên nếu muốn đọc hết thông tin thì hãy chú ý đến nó nhé.

Đó là tất cả những gì tôi muốn truyền tải trong dự án này. Cảm ơn vì đã đọc

~~~
Cảm ơn anh Đạt nhiều!!
~~~