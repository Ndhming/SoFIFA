Sang đến bước clean data, đây là bước clean data để phục vụ cho quá trình explore. Khi clean data chủ yếu để check xem các lỗi có trong tập dữ liệu hoặc là format lại tập dữ liệu cho phù hợp với việc phân tích. Các lỗi thường gặp:

Empty cells

Wrong format

Wrong data

Duplicate

Phần báo cáo này khá ngắn gọn bởi lẽ data được crawl xuống cũng đã khá clean rồi nên cũng không cần các thao tác clean data quá phức tạp khác.



Đầu tiên, tôi sử dụng các thư viện cần thiết như pandas, re, và os để hỗ trợ việc xử lý dữ liệu. Sau đó, dữ liệu được tải lên từ tệp sofifa_players.csv thông qua thư viện pandas, đồng thời lưu vào một dataframe (df) để thao tác. Sau khi tải lên, tôi kiểm tra tổng quan dữ liệu bằng phương thức df.info() để xem cấu trúc dữ liệu và phát hiện các lỗi hoặc giá trị bị thiếu.



Bước tiếp theo, thực hiện chuẩn hóa dữ liệu để đảm bảo tính chính xác. 

Trước tiên, tên các cột trong dataframe được làm sạch bằng cách loại bỏ khoảng trắng dư thừa, giúp tránh lỗi khi thao tác với dữ liệu. Đối với các cột về chiều cao và cân nặng, tôi loại bỏ các ký tự không cần thiết (ví dụ: "cm", "kg") và chuyển đổi tất cả về đơn vị cm và kg để đồng bộ. 

<img src="https://imgur.com/a/scrubbing-data-20BgG64">


Ngoài ra, dữ liệu về giá trị cầu thủ được chuẩn hóa bằng cách xây dựng hàm convert_currency(), trong đó các giá trị tiền tệ được chuyển từ dạng "€X triệu" hoặc "€X nghìn" thành số thực giúp thuận tiện hơn khi phân tích.


<img src="https://imgur.com/idHRkrl">



Sau đó, xây dựng hàm clean_numeric() để đảm bảo các cột dữ liệu số được định dạng chính xác, giúp loại bỏ các ký tự không mong muốn và chuyển đổi thành kiểu số nguyên hoặc số thực khi cần thiết.  Ngoài ra còn xác định và loại bỏ hoặc thay thế các bản ghi trùng lặp, các giá trị NaN, Null.





Cuối cùng, sau khi hoàn thành quá trình làm sạch, dữ liệu được lưu trữ lại dưới dạng tệp CSV để phục vụ cho các bước phân tích tiếp theo.



Tóm lại, quy trình xử lý dữ liệu này giúp chuẩn hóa dữ liệu từ SoFIFA, đảm bảo tính thống nhất về định dạng và tạo điều kiện thuận lợi cho các bước phân tích chuyên sâu EDA.

