﻿# 1. Giới thiệu

- Elasticsearch, Logstash, Kibana (ELK) được kết hợp lại để tạo lên một ứng dụng cung cấp sự kiện theo thời gian thực từ các nguồn dữ liệu có cấu trúc hoặc không cấu trúc.

# 2. Các thành phần

- Elasticsearch phụ trách tìm kiếm chuyên sâu và phân tích dữ liệu

- Logstash có nhiệm vụ làm nơi tập trung log và phân tích cú pháp

- Kibana hiển thị dữ liệu rất mạnh và đẹp.

# 3. Elasticsearch

- Elasticsearch là một bản phân phối, RESTful tìm kiếm và engine phân tích để giải quyết các trường hợp sử dụng ngày càng tăng.

- Truy vấn:
	- Elasticsearch cho phép bạn thực thi và kết hợp rất nhiều loại tìm kiếm: có cấu trúc, không cấu trúc, geo, metric theo cách bạn muốn.

- Phân tích:
	- Rất dễ tìm kiếm trong lượng dữ liệu ít, nhưng nếu có 1 tỷ dòng log thì thế nào? Elasticsearch cho phép bạn có cái nhìn để khai thác khuynh hướng và các mẫu trong dữ liệu.

- Tốc độ:
	- Elasticsearch thì rất nhanh, thực sự rất nhanh. Bạn có câu trả lời với dữ liệu thay đổi ngay lập tức.

- Khả năng mở rộng:
	- Bạn có thể chạy nó trên hàng trăm server với hàng petabyte dữ liệu.
	
- Vận hành dễ dàng:
	- Khả năng co giãn, Độ sẵn sàng cao
	- Dự đoán trước, tin cậy
	- Đơn giản, trong suốt
	
- Có thư viện cho các máy trạm
	- Elasticsearch sử dụng chuẩn RESTful APIs và JSON.
	
## Hiểu như nào là: A Distributed RESTful Search Engine
- Distributed and Highly Available Search Engine
	- Mỗi Index là full shard với một số cấu hình của shard
	- Mỗi shard có một hoặc nhiều replica
	- xử lý đọc và tìm kiến trên mõi replica shard.
	
- Multi Tenant with Multi Types
	- Hỗ trợ nhiều hơn một index
	- Hỗ trợ nhiều loại trên một index
	- Cấu hình index level (số shard, index storage)
	
- Various set of APIs
	- HTTP RESTful API
	- Native Java API
	- Tất cả API thực hiện thao tác node tự động mỗi khi định tuyến lại
	
- Document oriented
	- Không cần định nghĩa trước schema
	- Schema có thể được định nghĩa cho mỗi loại tùy vào quá trình indexing
	
- Tin cậy

- Tìm kiếm (gần) theo thời gian thực

- Xây dựng dựa trên Lucene
	- Mỗi shard là một Lucene index đầy đủ chức năng
	- Tất cả các ưu điểm của Lucene được khai phá thông qua cấu hình/plugin đơn giản.
	
- Hoạt động nhất quán
	- Document level hoạt động thống nhất, độc lập, lâu dài
	
- Open Source under the Apache License, version 2 (“ALv2”)
	
# Tham khảo
- [https://www.elastic.co/webinars/introduction-elk-stack](https://www.elastic.co/webinars/introduction-elk-stack)
- [https://github.com/elastic/elasticsearch](https://github.com/elastic/elasticsearch)
- 