# ViMs Dataset
300 Cụm văn bản tiếng Việt dùng cho tóm tắt đa văn bản

Tác giả: Nghiêm Quốc Minh

Đơn vị: Bộ môn Công nghệ Tri Thức, Đại học Khoa học Tự Nhiên Tp. HCM

Email liên hệ: nqminh@fit.hcmus.edu.vn

Đề tài SKHCN: Xây dựng công cụ tổng hợp tin tức tiếng Việt và ứng dụng

1. Quá trình xây dựng dữ liệu: 

   Dữ liệu được thu thâp một cách thủ công từ trang Google News, với số lượng 300 nhóm văn bản. Trong đó, mỗi nhóm văn bản sẽ có ít nhất là 5 bài, nhiều nhất là 10 bài. Các bài báo này được lấy từ những trang báo khá nổi tiếng và phổ biến ở Việt Nam như: Vnexpress, Dân Trí, Tuổi Trẻ, . . . Bộ ngữ liệu chứa các bài báo thuộc nhiều chuyên mục khác nhau, bao gồm: thế giới, Việt Nam (tin trong nước), kinh doanh, giải trí, và thể thao. Mỗi bài báo sẽ được lưu trữ trong cơ sở dữ liệu với các thông tin như sau: 

   * Title Tiêu đề bài báo. Ví dụ: “Giải mã bí ẩn máy bay rơi của EgyptAir”. 
   
   * Source Tên trang tin nguồn. Ví dụ: Vnexpress, Dân Trí, Tuổi Trẻ, . . .

   * URL Đường dẫn đến trang nguồn đăng bài báo gốc.

   * Published Date Ngày, giờ bài báo được đưa lên mạng.

   * Author Tác giả bài báo.

   * Tags Từ khóa của bài báo. Tùy từng trang tin nguồn, có trang có thông tin này, có trang không có.

   * Summary Tóm tắt bài báo do biên tập viên viết. Thông tin này thường nằm ở đầu bài báo, ngay sau tiêu đề của bài.

   * Content Nội dung bài báo. Nội dung này được lưu dưới dạng văn bản thô, đã loại bỏ các tag HTML, hình ảnh, và video.

   Sau khi kết thúc quá trình thu thập 300 nhóm văn bản, nhóm tiến hành xây dựng phần mềm để người gán nhãn có thể thực hiện tóm tắt các nhóm văn bản. Phần mềm đánh ngữ liệu được xây dựng dựa trên nền tảng mã nguồn mở MDSWriter. Mỗi cụm văn bản sẽ được thực hiện tóm tắt bởi hai người khác nhau, những người thực hiện tóm tắt là những người có kinh nghiệm và đang nghiên cứu về xử lý ngôn ngữ tự nhiên.

2. Thông tin dữ liệu:

   Thư mục original: Chứa 300 thư mục con chính là 300 cụm văn bản, trong mỗi cụm văn bản là các văn bản thuộc cùng 1 chủ đề. Có thể có 5 đến 10 bài cho mỗi cụm văn bản. Số lượng văn bản là 1,945.

   Thư mục summary: Chứa 300 thư mục con là 600 bản tóm tắt. Mỗi cụm văn bản đầu vào có 2 bản tóm tắt được tạo thủ công từ 2 người gán nhãn khác nhau với qui trình bảo đảm chất lượng bản tóm tắt tốt nhất có thể. Bộ ngữ liệu này có thể được sử dụng như là một nguồn ngữ liệu chuẩn để phục vụ quá trình đánh giá kết quả cho các nghiên cứu về tóm tắt đa văn bản trên Tiếng Việt.
