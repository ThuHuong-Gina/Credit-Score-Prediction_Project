# CREDIT SCORE_UNIVERSITY PROJECT
This is a Python project that I worked on in university on Bussiness Artificial Intelligent subject
## 1. Target
	- Enhance customer experience by reducing application processing time. 
 	- Improve the predictive capabilities of the credit scoring model using traditional methods to enhance the credit quality of installment loan customers, increase approval rates, and proactively manage bad debt. 
  	=> The 'Artificial Intelligence Credit Scoring' project provides a competitive advantage, increasing the bank's credibility in the market.
   
## 2. What is credit scoring?
This is a method implemented to assess the risk level of loan applicants based on both qualitative and quantitative factors, serving as the basis for determining credit limits for customers. Risk assessment of borrowers is conducted through statistical methods, data analysis, financial statement analysis, and balance sheet analysis. From this, certain indicators and maximum safe credit limits for a customer are determined, known as "scores," which banks use to evaluate and classify the credit risk of customers. This process involves analyzing past loan data to create an effective scoring model for customers.

## 3.The importance of credit scoring in the banking sector
	- Commercial banks always encounter various risks in their operations, such as credit risk, interest rate risk, liquidity risk, and foreign exchange risk. Among these, credit risk is the most significant as credit activities form the core operations of commercial banks, serving as a constant thread throughout their activities. Credit scoring and customer rating are conducted to assist commercial banks in:
  - Making credit decisions: determining credit limits, terms, interest rates, collateral, and approval or rejection of credit applications.
  - Monitoring and assessing creditworthy customers when credit accounts are outstanding. Customer ratings allow commercial banks to anticipate signs of deteriorating loan quality and take timely measures. From a portfolio management perspective, credit scoring and customer rating systems also serve the purpose of:
  - Developing marketing strategies to target less risky customers.
  - Estimating the amount of non-recoverable loans to set aside as credit loss provisions.
## 4. MODEL IMPLEMENTATION
### 4.1. Construct a comprehensive model
	With an ongoing stream of data from individual customers seeking substantial loans, which is continually updated through loan search websites or directly from Vietnamese commercial banks, the implementation of the Customer Credit Scoring process using artificial intelligence will streamline and expedite the customer credit rating process. Specifically, it involves applying classification methods to customer data to group customers. This procedure will consist of the following three stages:
Step 1: Gathering customer information.
Step 2: Utilizing artificial intelligence to perform credit scoring for individual customers.
Step 3: Generating a credit score report.

The process of collecting customer information will be assessed based on three primary criteria: Loan attributes, non-financial details, and customer financial information. This process is depicted in the following diagram.
        
The outcomes of the individual customer Credit Scoring process will be classified and specific determinations will be made for each category as outlined below:
	- Low-risk category: Offering loans with favorable terms.
	- Medium-risk category: Providing loans under standard conditions.
	- High-risk category: Possible exclusion from lending or lending with elevated interest rates or more stringent terms.
 ### 4.2. Model selection
 *Random Forest model:
	Step 1: Select random samples from the given dataset.
 	Step 2: Establish a decision tree for each sample, receiving predictions from each decision tree.
  	Step 3: Cast votes for each prediction.
   	Step 4: Choose the most frequently predicted result as the final prediction.
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


