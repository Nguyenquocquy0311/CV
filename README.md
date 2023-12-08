# Word detection for image
## Giới Thiệu
"Word detection for image" sử dụng các kiến trúc VGG16 và BLSTM để thực hiện nhiệm vụ nhận diện từ trong hình ảnh.

#### Thành viên nhóm:

- Nguyễn Quốc Quý
- Nguyễn Quốc Khánh
- Đỗ Đức Minh
## Bộ Dữ Liệu

Bộ dữ liệu được sử dụng để huấn luyện mô hình bao gồm hình ảnh từ ICDAR 2015 cho quá trình huấn luyện và ICDAR 2013 cho quá trình kiểm thử.

### Bộ Huấn Luyện
- Bộ huấn luyện bao gồm 1000 hình ảnh chứa văn bản được đặt ngẫu nhiên. Nói cách khác, các hình ảnh được chụp mà không có sự chú ý rõ ràng đến khu vực văn bản.

- Đáng chú ý, văn bản trên các hình ảnh này đa ngôn ngữ, đại diện cho nhiều ngôn ngữ khác nhau.

## Mô Hình

Mô hình được xây dựng bằng cách sử dụng các kiến trúc sau:

### VGG16
- VGG16 được sử dụng như một phần của kiến trúc mô hình. Đây là mạng nơ-ron tích chập sâu được biết đến với hiệu suất cao trong các nhiệm vụ phân loại hình ảnh.

### BLSTM (Bidirectional LSTM)
- Mạng Long Short-Term Memory có hướng kép (BLSTM) là một thành phần quan trọng khác của mô hình. Mạng BLSTM thường được sử dụng trong các nhiệm vụ chuỗi-qua-chuỗi, bao gồm xử lý ngôn ngữ tự nhiên và nhận diện chữ viết.