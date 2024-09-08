# Starbucks-Capstone-Project
![](https://lpcreativeco.com/wp-content/uploads/2017/08/combination-logo.jpg)

[Nguồn ảnh: lpcreativeco.com](https://lpcreativeco.com/wp-content/uploads/2017/08/combination-logo.jpg)

Starbukcs là một chuỗi cửa hàng cà phê quốc tế có trụ sở tại Seattle, Washington, Hoa Kỳ. Được thành lập vào năm 1971, Starbucks hiện nay là một trong những thương hiệu nổi tiếng trên thế giới trong lĩnh vực F&B.

Các nhóm đối tượng khách hàng mà Starbucks hướng đến khá rộng lớn, bao gồm sinh viên, nhân viên, v.v thậm chí gồm những người yêu thích không gian thoải mái để thư giãn và làm việc. Chính vì lý do đó, ngoài việc tập trung phát triển vào việc bán các mặt hàng thức uống và đồ ăn, Starbucks còn xây dựng mô hình kinh doanh tập trung vào các trải nghiệm khách hàng.

Vào khoảng năm 2018, Starbucks cùng với [Udacity](https://www.udacity.com/blog/2018/05/introducing-udacity-data-scientist-nanodegree-program.html) đã công bố bản ghi gồm các dữ liệu về các chiến dịch và thông tin khách hàng ấn danh để phục vụ cho các dự án nghiên cứu ở các trường đại học trên toàn thế giới. Bộ dữ liệu bao gồm 76.277 ưu đãi tiếp thị được gửi đến 17.000 người dùng trong 30 ngày.

Ở dự án này, chúng ta sẽ đi sâu vào **phân tích, và đưa ra các gợi ý về các chiến lược kinh doanh, quảng cáo phù hợp** dựa vào các thông tin về hành vi khách hàng của Starbucks và cách họ tương tác với các ưu đãi.

# ABOUT DATASET
Bộ dữ liệu gồm 3 file csv như sau:
## portfolio.csv

Bao gồm thông tin của 10 mã ưu đãi mà Starbucks đã thực hiện, trong đó:

+ **reward (int)**: số tiền (USD) mỗi khách hàng phải chi trả khi tham gia chiến dịch / ưu đãi.

+ **channels (list of strings)**: các kênh truyền thông được sử dụng trong ưu đãi.

+ **difficulty (int)**: số tiền (USD) Starbucks phải chi trả cho mỗi khách hàng khi tham gia ưu đãi.

+ **duration (int)**: là thời gian (ngày) thực hiện các ưu đãi.

+ **offer_type (string)**: kiểu ưu đãi, gồm giảm giá, cung cấp thông tin cá nhân, mua 1 tặng 1.

+ **id (string)**: mã ưu đãi.

## profile.csv

Gồm thông tin của các khách hàng như:

+ **id (string):** mã khách hàng .

+ **gender (string):** giới tính

+ **age (int)**: tuổi

+ **became_member_on (int):** ngày đăng ký thành viên

+ **income (float):** thu nhập hằng năm

## transcript.csv

Bao gồm các thông tin về giao dịch:

+ **person (string**): mã khách hàng.

+ **event (string)**: các sự kiện (*giao dịch* - transaction, *đã nhận được thông báo ưu đãi* - offer received, *đã hoàn thành ưu đãi* - offer completed, *đã xem ưu đãi* - offer viewed).

+ **value (dictionary containing strings)**: có thể là mã ưu đãi mà khách hàng sử dụng, hoặc là số tiền giao dịch cho sự kiên transaction.

+ **time (int)**: thời gian sử dụng ưu đãi của mỗi khách hàng (giờ) tính từ lúc Starbucks bắt đầu thực hiện bản ghi dữ liệu này.

