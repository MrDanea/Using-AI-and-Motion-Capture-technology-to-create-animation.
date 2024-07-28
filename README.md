# Ứng dụng AI vào công nghệ Motion Capture sản xuất Animation

- Lý do chọn đề tài:
  - Ngành công nghiệp văn hóa ở Việt Nam phát triển. Các chính sách đang được lới lỏng dần.
[![Watch the video](https://img.youtube.com/vi/Cx36Q5U17VA/0.jpg)](https://www.youtube.com/watch?v=Cx36Q5U17VA)
  - Công nghệ mới, tuy đã được thương mại gần đây bởi công ty MOVE AI bên nước ngoài nhưng ở Việt Nam hoàn toàn có cơ hội phát triển.
- Mô tả sơ bộ: 
![Model](https://drive.google.com/uc?export=view&id=1H6q9aOxhaWW78mrsWdVEAxfKqC4-RsyT)
  - Phần Camera có hai phương án lựa chọn:
    - Dùng 1-2 camera trên điện thoại, sử dụng phần mềm để đưa dữ liệu về máy chủ.
    - Sử dụng 2 module camera và một MCU để gửi cùng lúc tới máy chủ.
  - Phương thức truyền tải từ Camera tới máy chủ có 2 lựa chọn:
    - Sử dụng RTMP/Dash để gửi thông qua Internet.
    - Sử dụng Ethernet nối trực tiếp tới máy chủ.
    - Khả năng vẫn còn cách khác nhưng chưa biết, hình như nối cáp trực tiếp luôn.
  - Cách bắt chuyển động có 2 phương án:
    - Chế độ quay video rồi gửi từ Camera tới máy chủ. Ưu điểm là không cần phải đồng bộ hóa giữa các Camera, nhược điểm là chất lượng hình ảnh không bằng chụp
    - Chế độ chụp liên tiếp. Ưu điểm alf chất lượng hình ảnh tốt. Nhược điểm là cần phải đồng bộ thời điểm chụp của các máy ảnh.
  - Sử dụng Cloud làm môi trường để huấn luyện AI, tuy nhiên chi phí khá cao nhưng nếu ai chưa đăng ký AWS, Azure thì vẫn còn miễn phí 1 năm.
  - Dùng model YOLO để nhận diện, nếu thương mại hóa sẽ mất phí (chưa rõ bao nhiêu).
  - Sử dụng HTTPstreaming để đẩy data về 
  - Sản phẩm cuối cùng sẽ là các file USD, MP4, FBX,... những file này phải export được vào các công cụ 3d như blender, UE5, Unity,... để tạo chuyển động Animation. Ngoài ra các công cụ trên đều có tính năng Livelink, Tính năng này cho phép truyền trực tiếp dữ liệu vào tuy nhiên nếu thương mại sẽ có chi phí tương đối cao hơn nữa khả năng sẽ cần phải thiết kế lại mô hình ban đầu.
- Những việc phải làm:
  - Tìm ra một giải pháp quản lý dự án.
  - Cân nhắc giữa các phương án nêu trên nhằm tối thiểu chi phí.
  - Phân công mỗi người 2-3 mảng phụ trách. Bao gồm (Cloud + Training AI, Desktop Apps, Mobile apps(Design Hardware for Camera), Analyze the structure of mp4, usd, fbx files), ngoài ra tìm hiểu thêm về livelink.
  - Cách viết báo cáo tiến độ.


