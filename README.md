# CREDIT SCORE_UNIVERSITY PROJECT
This is a Python project that I worked on in university on Bussiness Artificial Intelligent subject
## 1. Mục tiêu  
	- Cải thiện trải nghiệm của khách hàng trong việc giảm thiểu thời gian xét duyệt hồ sơ. 
	- Cải thiện khả năng dự đoán của mô hình chấm điểm theo phương pháp truyền thống, tăng chất lượng tín dụng của khách hàng vay trả góp, tăng tỷ lệ phê duyệt trả góp và chủ động kiểm soát nợ xấu. 
	=> Dự án “Chấm điểm tín dụng bằng trí tuệ nhân tạo” mang đến lợi thế cạnh tranh, tăng tỷ lệ tín nhiệm của ngân hàng trên thị trường.
## 2. Chấm điểm tín dụng là gì?
Đây là phương pháp được thực hiện để đánh giá mức độ rủi ro của khách hàng vay vốn trên cơ sở định tính và định lượng, làm căn cứ để xác định giới hạn tín dụng cho khách hàng. Trên cơ sở đánh giá mức độ rủi ro của người đi vay thông qua các phương pháp thống kê, nghiên cứu dữ liệu, phân tích bảng báo cáo tài chính, bảng cân đối kế toán…từ đó đưa ra những chỉ số, giới hạn tín dụng an toàn tối đa đối với một khách hàng, đó được gọi là “điểm” để các ngân hàng căn cử đánh giá, xếp loại rủi ro tín dụng của khách hàng. Từ việc phân tích những dữ liệu về các khoản vay trong quá khứ để tạo dựng một hình mẫu chấm điểm hiệu quả cho khách hàng. 
## 3.Sự cần thiết của chấm điểm tín dụng trong ngân hàng
	- Các ngân hàng thương mại luôn đối mặt với những rủi ro trong quá trình hoạt động của mình như rủi ro tín dụng, rủi ro lãi suất, rủi ro thanh khoản, rủi ro về ngoại hối… Trong đó rủi ro tín dụng là đáng chủ trọng nhất, vì hoạt động tín dụng là hoạt động chủ yếu nhất của các ngân hàng thương mại, là sợi chỉ đỏ xuyên suốt quá trình hoạt động của các ngân hàng thương mại. Việc chấm điểm tín dụng và xếp hạng khách hàng được thực hiện nhằm hỗ trợ NHCV trong việc:
	- Ra quyết định cấp tín dụng: xác định hạn mức tín dụng, thời hạn, mức lãi suất, biện pháp bảo đảm tiền vay, phê duyệt hay không phê duyệt. 
	- Giảm sát và đánh giá khách hàng tín dụng khi khoản tín dụng đang cò dư nợ; Hạng khách hàng cho phép NHCV lường trước những dấu hiệu cho thấy khoản vay đang có chất lượng xấu đi và có những biện pháp đối phó kịp thời. Xét trên góc độ quản lý toàn bộ danh mục tín dụng, hệ thống chấm điểm tín dụng và xếp hạng khách hàng còn nhằm mục đích:
	- Phát triển chiến lược marketing nhằm hướng tới các khách hàng có ít rủi ro hơn 
	- Ước lượng mức vốn đã cho vay sẽ không thu hồi được để trích lập dự phòng tổn thất tín dụng.
## 4. TRIỂN KHAI MÔ HÌNH
### 4.1. Xây dựng mô hình chung 
	Với nguồn dữ liệu khách hàng cá nhân có nhu cầu vay vốn với số lượng lớn được cập nhật liên tục qua các trang web tìm kiếm nguồn vay hay trực tiếp tại các ngân hàng thương mại VN. Với việc triển khai quá trình XHTD cho khách hàng bằng trí tuện nhân tạo thì quy trình xếp hạng tín dụng cho khách hàng sẽ nhanh chóng và tuận tiện hơn. Cụ thể là sử dụng phương pháp phân lớp - classifications áp dụng trên thông tin dữ liệu của khách vay để phân loại nhóm khách hàng. Quy trình này sẽ được làm theo 3 bước sau:
	Bước 1: Thu thập thông tin khách hàng
	Bước 2: Thực hiện chấm điểm tín dụng khách hàng cá nhân bằng trí tuệ nhân tạo
	Bước 3: Báo cáo chấm điểm
	- Với quá trình thu thập thông tin khách hàng sẽ được đánh giá qua 3 tiêu trí chính: Đặc điểm khoản vay, thông tin phi tài chính và thông tin tài chính của khách hàng. Quá trình này được thể hiện qua sơ đồ sau:
        
Kết quả cảu quá trình XHTD khách hàng cá nhân sẽ được đánh giá phân lớp và đưa ra các kết luận cho từng nhóm như sau:
	- Nhóm rủi ro thấp: Cho vay với chính sách ưu đãi.
	- Nhóm rủi ro trung bình: Cho vay với điều kiện bình thường.
	- Nhóm rủi ro cao: Có thể không cho vay hoặc cho vay nhưng áp dụng lãi suất cao hay cho vay với điều kiện khắt khe hơn.
 ### 4.2. Lựa chọn mô hình 
 *Mô hình random forest:
	Bước 1: Chọn các mẫu ngẫu nhiên từ tập dữ liệu đã cho.
	Bước 2: Thiết lập cây quyết định cho từng mẫu, nhận kết quả dự đoán từ mỗi quyết định cây.
	Bước 3: Bỏ phiếu cho mỗi kết quả dự đoán.
	Bước 4: Chọn kết quả được dự đoán nhiều nhất là dự đoán cuối cùng.
### 4.3. Các nhân tố được xem xét khi xếp hạng tín dụng cá nhân-lựa chọn các biến
	Để áp dụng vào bài toán XHDT cho khách hàng thì trước hết ta cần xây dựng được các chỉ tiêu đánh giá dựa vào các căn cứ xác định mức cho vay dưới đây:
	- Mức vốn của khách hàng tham gia vào dự án, phương án kinh doanh, sản xuất, dịch vụ, đời sống.
	- Tỷ lệ cho vay tối đa so với giá trị tài sản bảo đảm tiền vay theo quy định về bảo đảm tiền vay của ngân hàng. 
	- Khả năng hoàn trả nợ của khách hàng. 
	- Khả năng nguồn vốn của mỗi ngân hàng và không được vượt quá định mức cho vay được ủy quyền bởi tổng giám đốc Ngân hàng cho vay
	=> Dựa vào các căn cứ cho vay trên của ngân hàng ta đưa được các chi tiêu cụ thể để đánh giá và xác định mức cho vay như sau:
#### Chỉ tiêu phi tài chính:
+ Độ tuổi
+ Trình độ học vấn
+ Số lao động trong gia đình
+ Thời gian gắn bó với công việc hiện tại
+ Số lượng nguồn thu tài chính
#### Chỉ tiêu tài chính:
+ Thu nhập cố định mỗi tháng
+ Giá trị tài sản bảo đảm (nhà, xe, đất, …)
+ Tài khoản tiết kiệm
+ Số dư nợ hiện có
#### Đặc điểm khoản vay:
+ Lãi suất
+ Thời hạn
+ Tỷ lệ khoản vay 
+ Phương thức trả

### 4.4. Hệ thống xếp hạng
Mô hình này chú trọng nhiều hơn về khả năng trả nợ với 8 chỉ tiêu đánh giá, trong khi đó đặc điểm thân nhân chỉ có 4 chỉ tiêu đánh giá. Chương trình sẽ kiểm tra tính hợp lý của dữ liệu theo nguyên tắc kiểm soát chỉ số và chỉ ra những điểm cần xem xét lại khi phát hiện có sự không hợp lý về chỉ tiêu pháp lý, chỉ tiêu chấm điểm, tổng điểm và xếp hạng của khách hàng. Hệ thống ký hiệu xếp hạng cá nhân có các mức giảm từ AAA đến D như trình bày trong bảng sau. Căn cứ vào tổng điểm tối đa giảm dần từ 100 điểm của từng cá nhân (đã quy đổi theo trọng số như trên) để xếp hạng tương ứng.
![image](https://github.com/ThuHuong-Gina/Credit-Score-Prediction_Project/assets/141025228/c9bcb898-677c-4d47-88a2-ea0dacad47c7)


