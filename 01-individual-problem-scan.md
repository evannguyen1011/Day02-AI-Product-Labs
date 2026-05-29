# paint point mà em nhận thấy được trong khóa học:
| # | Lăng kính | Problem quan sát được | AI đang đau? | Dấu hiệu thật |
|---|-----------|-----------------------|--------------|---------------|
| 1 | Tốn thời gian | Nhà ăn chuẩn bị thiếu đồ, học viên đến muộn thường xuyên bị hết món, phải đợi nấu lại hoặc nhịn ăn. | Học viên, Đầu bếp canteen | Xảy ra hàng ngày vào khung giờ 11h45 - 12h30. |
| 2 | Lặp lại | Quá nhiều thủ tục nhập học, giấy tờ, quy định điểm danh phức tạp khiến người mới bối rối, hỏi đi hỏi lại. | Học viên mới, Phòng đào tạo | Mất 2-3 ngày đầu khóa để giải quyết; fanpage/group lớp bị spam cùng một câu hỏi. |
| 3 | AI có thể tốt hơn | Lượng kiến thức khổng lồ khiến học viên không kịp tiêu hóa, gặp khó khăn khi tự cài đặt môi trường và quản lý lịch học/nghỉ ngơi. | Học viên | Thức khuya đến 2-3h sáng; nhiều học viên nợ bài tập ngay từ tuần thứ 2. |
| 4 | Pain từ người khác | Học viên ngoại tỉnh khó tìm trọ quanh trường, dễ bị "chém giá" hoặc thuê phải phòng không đúng mô tả. | Học viên mới | Mất 3-5 ngày đi tìm trực tiếp; chi phí bị đội lên 20-30% so với giá thị trường. |
| 5 | Lặp lại | Khó khăn và mất thời gian trong việc tìm kiếm, kết nối đồng đội để lập nhóm làm Assignment/Project có cùng trình độ. | Học viên, Lớp trưởng | Mất cả tuần đầu khóa để ổn định danh sách; cuối kỳ xuất hiện nhiều nhóm "gánh tạ". |
| 6 | AI có thể tốt hơn | Học viên bị sụt giảm phong độ, âm thầm "burnout" và muốn bỏ học giữa chừng do áp lực học tập quá nặng nề. | Học viên, Giảng viên | Tần suất đăng nhập LMS giảm 50%; tỷ lệ nộp muộn tăng cao sau tuần thứ 4. |
| 7 | AI có thể tốt hơn | Mạng nội bộ của trường bị nghẽn, load chậm hoặc rớt mạng liên tục vào các khung giờ cao điểm làm bài Lab. | Toàn bộ học viên, Bộ phận IT | Mất 15-20 phút chỉ để kéo (pull) một thư viện code; nghẽn băng thông diện rộng. |

# top3:

| 1 | Tốn thời gian | Nhà ăn chuẩn bị thiếu đồ, học viên đến muộn thường xuyên bị hết món, phải đợi nấu lại hoặc nhịn ăn. | Học viên, Đầu bếp canteen | Xảy ra hàng ngày vào khung giờ 11h45 - 12h30. |

| 4 | Pain từ người khác | Học viên ngoại tỉnh khó tìm trọ quanh trường, dễ bị "chém giá" hoặc thuê phải phòng không đúng mô tả. | Học viên mới | Mất 3-5 ngày đi tìm trực tiếp; chi phí bị đội lên 20-30% so với giá thị trường. |

| 7 | AI có thể tốt hơn | Mạng nội bộ của trường bị nghẽn, load chậm hoặc rớt mạng liên tục vào các khung giờ cao điểm làm bài Lab. | Toàn bộ học viên, Bộ phận IT | Mất 15-20 phút chỉ để kéo (pull) một thư viện code; nghẽn băng thông diện rộng. |


## Problem Card #1 – Canteen Supply Shortage
Bài toán một câu:
Học viên đến muộn thường xuyên bị hết món do nhà ăn chuẩn bị thiếu đồ, dẫn đến việc phải đợi nấu lại hoặc nhịn ăn, gây lãng phí thời gian và ảnh hưởng sức khỏe.

Actor:
Học viên (người ăn), Đầu bếp canteen (người chuẩn bị và nấu nướng).

Thời điểm / bối cảnh:
Hàng ngày, vào khung giờ cao điểm từ 11h45 - 12h30.

Current workflow:

Đầu bếp ước lượng số lượng suất ăn dựa trên trực giác hoặc số liệu lịch sử cũ.

Nấu ăn theo số lượng đã ước lượng.

Học viên đến xếp hàng, lấy đồ ăn và thanh toán.

Học viên đến muộn phát hiện hết món, phải đợi nhà bếp nấu món mới hoặc chấp nhận nhịn ăn/đi ăn ngoài.

Bottleneck:
Bước 1 – Đầu bếp không có số liệu chính xác về số lượng học viên sẽ đến ăn theo thời gian thực hoặc theo ngày (ví dụ: ngày có lịch thi, số lượng đi học thực tế biến động).

Impact:
Học viên mất thêm 15-20 phút đợi nấu lại hoặc bị đói, giảm hiệu suất học tập buổi chiều. Nhà bếp bị động trong việc chuẩn bị nguyên liệu, dễ gây lãng phí hoặc mất doanh thu.

Success metric:
Giảm tỷ lệ học viên bị hết món xuống dưới 5%, thời gian chờ đợi của học viên muộn giảm về 0.

Non-AI alternative:
Học viên đăng ký suất ăn thủ công qua Google Form trước 10h sáng hàng ngày. Tuy nhiên, cách này phiền phức và tỷ lệ học viên quên điền rất cao.

AI hypothesis:
AI dự đoán số lượng suất ăn cần chuẩn bị theo ngày và theo khung giờ bằng cách phân tích dữ liệu lịch sử lịch học, lịch thi, thời tiết và dữ liệu điểm danh thực tế từ phòng đào tạo.

Phán đoán ban đầu:
Data / Model.

## Problem Card #4 – Accommodation Searching Pain
Bài toán một câu:
Học viên ngoại tỉnh gặp nhiều khó khăn, mất thời gian khi tìm phòng trọ quanh trường, dễ bị lừa đảo, "chém giá" hoặc thuê phải phòng không đúng với mô tả trên mạng.

Actor:
Học viên mới (đặc biệt là học viên ngoại tỉnh).

Thời điểm / bối cảnh:
Khoảng 1-2 tuần trước khi khóa học mới chính thức khai giảng.

Current workflow:

Học viên tìm thông tin phòng trọ trên các group Facebook hoặc website bất động sản.

Lọc thông tin, liên hệ với chủ nhà/môi giới.

Đi đến tận nơi (mất 3-5 ngày) để xem phòng và xác thực thực tế.

Chốt thuê phòng và đặt cọc.

Bottleneck:
Bước 1 và Bước 3 – Thông tin trên mạng bị nhiễu, nhiều bài đăng giả mạo hoặc đẩy giá bừa bãi, khiến học viên mất quá nhiều công sức đi xác thực trực tiếp.

Impact:
Học viên mất từ 3-5 ngày đi tìm phòng trực tiếp; chi phí thuê trọ bị đội lên 20-30% so với giá trị thị trường thực tế; gây stress lớn trước khi nhập học.

Success metric:
Học viên tìm được phòng ưng ý, đúng mô tả trong vòng dưới 2 ngày; chi phí thuê đúng giá thị trường.

Non-AI alternative:
Phòng đào tạo hoặc Hội sinh viên lập một danh sách (Excel) các nhà trọ uy tín quanh trường để hỗ trợ người mới. Nhược điểm: Danh sách nhanh bị lỗi thời, tốn công duy trì thủ công.

AI hypothesis:
Xây dựng bot tự động cào (crawl) dữ liệu phòng trọ, dùng AI để lọc/phân loại, phát hiện các bài đăng có dấu hiệu lừa đảo/ảo giá, và đề xuất phòng phù hợp dựa trên khoảng cách và ngân sách của học viên.

Phán đoán ban đầu:
Data / Integration.

## Problem Card #7 – Lab Session Network Congestion
Bài toán một câu:
Mạng nội bộ của trường liên tục bị nghẽn, rớt mạng vào các khung giờ cao điểm làm bài Lab, khiến học viên tốn rất nhiều thời gian chỉ để tải hoặc kéo thư viện code.

Actor:
Toàn bộ học viên đang thực hành, Bộ phận IT của trường.

Thời điểm / bối cảnh:
Khung giờ cao điểm của các buổi làm bài Lab hoặc khi có nhiều lớp cùng thực hành code đồng thời.

Current workflow:

Giảng viên giao bài Lab / Project cho học viên.

Học viên đồng loạt chạy lệnh kết nối internet để kéo thư viện (pip install, npm install, git pull...).

Băng thông mạng trường bị quá tải.

Mạng bị nghẽn, học viên phải đợi hoặc hủy lệnh để chạy lại.

Bottleneck:
Bước 2 & Bước 3 – Hàng trăm máy tính cùng gửi yêu cầu tải các file có dung lượng lớn từ server quốc tế cùng một lúc, gây thắt nút cổ chai băng thông.

Impact:
Mất từ 15-20 phút chỉ để kéo một thư viện code cơ bản. Giảm thời gian làm bài thực tế của học viên, gây ức chế và làm gián đoạn mạch tiến độ của buổi học.

Success metric:
Thời gian kéo thư viện và tải tài liệu giảm xuống dưới 1 phút trong mọi khung giờ cao điểm.

Non-AI alternative:
Nâng cấp gói băng thông mạng của trường (tốn chi phí lớn) hoặc cấu hình một máy chủ Proxy/Local Cache trong mạng nội bộ để lưu trữ sẵn các thư viện phổ biến.

AI hypothesis:
AI giám sát lưu lượng mạng theo thời gian thực, tự động dự đoán các đợt cao điểm dựa trên lịch học bài Lab để điều phối, giới hạn băng thông (QoS) thông minh hoặc tự động kích hoạt bộ nhớ đệm (caching) cho các gói dữ liệu được yêu cầu nhiều nhất.

Phán đoán ban đầu:
System / Infrastructure.

# bieu do
## bieu do case 1
CURRENT STATE — 45 phút
+--------------------+     +--------------------+     +--------------------+     +--------------------+
| 1. Ước lượng suất  | --> | 2. Nấu ăn theo     | --> | 3. Học viên        | --> | 4. Đến muộn bị     |
|    ăn (5 phút)     |     |    ước lượng (20') |     |    xếp hàng (15')  |     |    hết món (5') [R]|
+--------------------+     +--------------------+     +--------------------+     +--------------------+
                                                                                            |
                                                                                            v
FUTURE STATE — 23 phút                                                                 [R] = Bottleneck
+--------------------+     +--------------------+     +--------------------+
| 1. AI dự đoán      | --> | 2. Đầu bếp review  | --> | 3. Nấu ăn theo     |
|    số lượng (1')   |     |    số lượng (2') [G|     |    AI đề xuất (20')|
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
                                                      [G] = Human boundary
                                                      Fallback: AI lệch -> Nấu theo số cũ

## bieu do case 4
CURRENT STATE — 5 ngày
+--------------------+     +--------------------+     +--------------------+
| 1. Tìm phòng trên  | --> | 2. Lọc thông tin   | --> | 3. Đi thực tế      |
|    FB/Web nhiễu [R]|     |    & liên hệ (1 ng)|     |    xác thực (3 ng) |
+--------------------+     +--------------------+     +--------------------+
          |
          v
   [R] = Bottleneck

FUTURE STATE — 1.5 ngày
+--------------------+     +--------------------+     +--------------------+
| 1. Bot crawl & AI  | --> | 2. Học viên lướt   | --> | 3. Đi chốt phòng   |
|    lọc tin giả (2h)|     |    list sạch (2h)[G|     |    thực tế (1 ngày)|
+--------------------+     +--------------------+     +--------------------+
                                                               |
                                                               v
                                                      [G] = Human boundary
                                                      Fallback: App lỗi -> Tự đi tìm tay

## bieu do case 7
CURRENT STATE — 35 phút
+--------------------+     +--------------------+     +--------------------+     +--------------------+
| 1. Giảng viên      | --> | 2. Đồng loạt chạy  | --> | 3. Nghẽn mạng,     | --> | 4. Thử lại/Đợi     |
|    giao bài Lab (5')|    |    lệnh kéo lib (5')|    |    rớt gói (20')[R]|     |    nhả mạng (5')   |
+--------------------+     +--------------------+     +--------------------+     +--------------------+
                                                                                            |
                                                                                            v
FUTURE STATE — 6 phút                                                                  [R] = Bottleneck
+--------------------+     +--------------------+     +--------------------+
| 1. Giảng viên      | --> | 2. AI tự động điều | --> | 3. Local Cache/    |
|    giao bài Lab (5')|    |    phối mạng (0.5')|     |    Kéo code mượt(0.5)|
+--------------------+     +--------------------+     +--------------------+