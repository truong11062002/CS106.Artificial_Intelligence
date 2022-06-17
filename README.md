<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: 5;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<!-- Title -->
<h1 align="center"><b>CS106.M21 Trí tuệ nhân tạo</b></h1>



## BẢNG MỤC LỤC
* [ Giới thiệu môn học](#gioithieumonhoc)
* [Quá trình môn học](#quatrinh)
* [ Giảng viên hướng dẫn](#giangvien)
* [ Thành viên nhóm](#thanhvien)
* [ Đồ án môn học](#doan)
## GIỚI THIỆU MÔN HỌC
<a name="gioithieumonhoc"></a>
* **Tên môn học**: Trí tuệ nhân tạo
* **Mã môn học**: CS106
* **Lớp học**: CS106.M21
* **Ngày bắt đầu**: 21/02/2022
* **Ngày kết thúc**: 11/06/2022
* **Năm học**: 2021-2022
## QUÁ TRÌNH MÔN HỌC
<a name ="quatrinh"></a>
### 1.Trí tuệ nhân tạo


<a name ="colab"></a>
### 2.COLAB ASSSIGNMENTS


<a name ="QT"></a>
### 3.QT IN CLASS

## GIẢNG VIÊN HƯỚNG DẪN
<a name="giangvien"></a>
* PGS.TS. **Lương Ngọc Hoàng** - *hoangln@uit.edu.vn*

## THÀNH VIÊN NHÓM
<a name="thanhvien"></a>
| STT    | MSSV          | Họ và Tên              | Github                                               | Email                   |
| ------ |:-------------:| ----------------------:|-----------------------------------------------------:|-------------------------:
| 1      | 20522087      | Nguyễn Nhật Trường     |https://github.com/truong11062002                     |20522087@gm.uit.edu.vn   |
| 2      | 20520481      | Lê Trương Ngọc Hải     |https://github.com/letruongngochai                    |20520481@gm.uit.edu.vn   |
| 3      | 20520355      | Lê Thị Phương Vy       |https://github.com/Ceci-june                          |20520355@gm.uit.edu.vn   |
| 4      | 20520309      | Lại Chí Thiện          |https://github.com/laichithien                        |20520309@gm.uit.edu.vn   |
## ĐỒ ÁN MÔN HỌC
<a name="doan"></a>
Tên đồ án: Traffic Signal Control
### Những chỉnh sửa trong source code (nhằm để tương thích với phiên bản hiện tại trên Google Colaboratory) ở các file sau:
+ anon_env.py: sửa "import engine" thành "import pyttsx3", trước đó phải "pip install pyttsx3"
+ simple_dqn_agent.py + network_agent.py: sửa "from keras.optimizers import RMSprop" thành "from tensorflow.keras.optimizers import RMSprop"
+ network_agent: sửa "from keras.engine.topology import Layer" thành "from tensorflow.keras.layers import Layer"
### Để chạy một experiment: python -O runexp.py
### Mô tả các file trong source code:
+ agent.py: Một lớp trừu tượng của các agent khác nhau
+ network_agent.py: Agent PressLight
+ runexp.py: Chạy pipeline với những dòng giao thông khác nhau. File này chứa cấu hình cơ bản của phương pháp. Mọi thông tin chi tiết hơn được mô tả trong config.py
+ config.py: Toàn bộ cấu hình của đồ án này. Một số tham số sẽ được thay thế trong runexp.py, còn lại thì chỉ thay đổi trong file này.
+ pipeline.py: File chứa toàn bộ quy trình: Khởi tạo một môi trường -> Chạy giả lập với một khoảng thời gian nhất định (1 vòng) -> Xây dựng mẫu dữ liệu từ raw log data -> Cập nhật mô hình -> Model pooling
+ generator.py: Một trình tạo để load mô hình, khởi động môi trường giả lập, tiến hành mô phỏng và ghi lại kết quả.
+ anon_env.py: Định nghĩa môi trường giả lập để tương tác với bộ giả lập và thu được đặc trưng.
+ construct_sample.py: Xây dựng mẫu dữ liệu huấn luyện từ dữ liệu gốc. Chọn các đặc trưng trạng thái mong muốn trong cấu hình và tính toán reward trung bình/tức thì tương ứng với thời gian đo cụ thể
+ updater.py: Định nghĩa một lớp của bộ cập nhật để cập nhật mô hình
