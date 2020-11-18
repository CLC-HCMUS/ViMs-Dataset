# ViMs Dataset
300 news clusters for Vietnamese abstractive multi-document summarization

Author: Nghiem Quoc Minh et al., 2016

Institute: Faculty of Information Technology, HCMC University of Science, Vietnam

Email: nqminh@fit.hcmus.edu.vn

Please cite to the following journal when using the dataset:

```
   @article{tran2020vims,
     title={ViMs: a high-quality Vietnamese dataset for abstractive multi-document summarization},
     author={Tran, Nhi-Thao and Nghiem, Minh-Quoc and Nguyen, Nhung TH and Nguyen, Ngan Luu-Thuy and Van Chi, Nam and Dinh, Dien},
     journal={Language Resources and Evaluation},
     volume={54},
     number={4},
     pages={893--920},
     year={2020},
     publisher={Springer}
}
```

This work was supported by the Ho Chi Minh City Department of Science and Technology, Grant Numbers 15/2016/HÐ-SKHCN

#### Data construction process:

In this work, we aim to have 300 clusters of documents extracted from news. To this end, we made use of the Vietnamese language version of Google News. Due to the copyright issue, we did not collect articles from every source listed on Google News, but limited to some sources that are open for research purposes. The collected articles belong to five genres: world news, domestic news, business, entertainment, and sports. Every cluster contains from four to ten news articles. Each article is represented by the following information: the title, the plain text content, the news source, the date of publication, the author(s), the tag(s) and the headline summary.

After that, two summaries are created for each cluster (produced in the first subtask above) by two distinguished annotators using the MDSWriter system (Meyer, Christian M., et al. "MDSWriter: Annotation tool for creating high-quality multi-document summarization corpora." Proceedings of ACL-2016 System Demonstrations). These annotators are Vietnamese native speakers and they are undergraduate students or graduate students. Most of them know about natural language processing. The full annotation process consists of seven steps that must be done sequentially from the first to the seventh one.

#### Data information:

Original folder: Containing 300 subdirectories which are 300 news clusters. Articles (documents) in each cluster belong to a similar topic and there are from four to ten of them. The number of articles is 1,945.

Summary folder: Contains 300 subdirectories which are 600 final summaries. Every input cluster has two manual abstract summaries from two distinguished annotators. ViMs can be used for both implementing and evaluating supervised machine learning-based systems for Vietnamese abstractive multi-document summarization.

S3_summary folder: Contains 300 subdirectories including 600 ''best sentence selection'' summaries, the result of step 3 -- best sentence selection step. Sentences in a group are separated from others by a blank line. The most important sentence is marked as 1 while 0 is the label for others.


-----------------------------------------------------------------------------------------------------------------------------


# Bộ dữ liệu ViMs
300 Cụm văn bản tiếng Việt dùng cho tóm tắt đa văn bản

Tác giả: nhóm tác giả Nghiêm Quốc Minh

Đơn vị: Bộ môn Công nghệ Tri Thức, Đại học Khoa học Tự Nhiên Tp. HCM

Email liên hệ: nqminh@fit.hcmus.edu.vn

```
   @article{tran2020vims,
     title={ViMs: a high-quality Vietnamese dataset for abstractive multi-document summarization},
     author={Tran, Nhi-Thao and Nghiem, Minh-Quoc and Nguyen, Nhung TH and Nguyen, Ngan Luu-Thuy and Van Chi, Nam and Dinh, Dien},
     journal={Language Resources and Evaluation},
     volume={54},
     number={4},
     pages={893--920},
     year={2020},
     publisher={Springer}
}
```

Đề tài SKHCN: Xây dựng công cụ tổng hợp tin tức tiếng Việt và ứng dụng

#### Quá trình xây dựng dữ liệu: 

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

#### Thông tin dữ liệu:

Thư mục original: Chứa 300 thư mục con chính là 300 cụm văn bản, trong mỗi cụm văn bản là các văn bản thuộc cùng 1 chủ đề. Có thể có 5 đến 10 bài cho mỗi cụm văn bản. Số lượng văn bản là 1,945.

Thư mục summary: Chứa 300 thư mục con là 600 bản tóm tắt. Mỗi cụm văn bản đầu vào có 2 bản tóm tắt được tạo thủ công từ 2 người gán nhãn khác nhau với qui trình bảo đảm chất lượng bản tóm tắt tốt nhất có thể. Bộ ngữ liệu này có thể được sử dụng như là một nguồn ngữ liệu chuẩn để phục vụ quá trình đánh giá kết quả cho các nghiên cứu về tóm tắt đa văn bản trên Tiếng Việt.

Thư mục S3_summary: Chứa 300 thư mục con gồm 600 bản tóm tắt, là kết quả của bước chọn câu quan trọng. Các nhóm chứa các câu mang nghĩa tương đương nhau, cách nhau bởi 1 dòng trống. Câu quan trọng nhất được chọn từ một nhóm có nhãn 1, các câu còn lại mang nhãn 0.  
