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
Những chỉnh sửa trong source code (nhằm để tương thích với phiên bản hiện tại trên Google Colaboratory) ở các file sau:
+ anon_env.py: sửa "import engine" thành "import pyttsx3", trước đó phải "pip install pyttsx3"
+ simple_dqn_agent.py + network_agent.py: sửa "from keras.optimizers import RMSprop" thành "from tensorflow.keras.optimizers import RMSprop"
+ network_agent: sửa "from keras.engine.topology import Layer" thành "from tensorflow.keras.layers import Layer"
