Mình đã đọc nội dung PDF của bạn , dưới đây là phiên bản **định dạng Markdown để bạn đưa thẳng vào README.md trên GitHub**.

Bạn chỉ cần copy toàn bộ phần dưới:

---

# stego-mfcc-encode

**Audio Steganography using MFCC Features**

## Giới thiệu

Bài lab thực hiện kỹ thuật giấu tin trong âm thanh sử dụng đặc trưng MFCC (Mel-Frequency Cepstral Coefficients).
Sinh viên sẽ thực hiện trích xuất MFCC, giấu thông điệp vào MFCC và đánh giá chất lượng âm thanh sau khi giấu tin.

---

# 1. Mục đích

* Hiểu và thực hành kỹ thuật giấu tin trong âm thanh sử dụng MFCC.
* Thực hành tạo thông điệp bí mật và giấu vào tín hiệu âm thanh.
* Nắm được nguyên lý steganography trong âm thanh dựa trên đặc trưng MFCC.

---

# 2. Yêu cầu

Sinh viên cần:

* Hiểu nguyên lý giấu tin trong âm thanh bằng MFCC.
* Thực hiện các bước:

  * Trích xuất MFCC
  * Giấu tin vào MFCC
  * Đánh giá kết quả bằng MSE
* So sánh sự khác biệt giữa âm thanh gốc và âm thanh đã giấu tin.

---

# 3. Kịch bản bài lab

Trong bài lab này, bạn đóng vai trò **người gửi (sender)** muốn giấu một thông điệp bí mật vào file âm thanh WAV.

## Đầu vào

* `sample.wav`

## Đầu ra

* `stego_audio.wav` – Âm thanh đã giấu tin
* `mfcc_stego.npy` – MFCC sau khi giấu tin
* `waveform_comparison.png` – Biểu đồ so sánh dạng sóng
* `waveform_report.txt` – Báo cáo MSE

---

# 4. Chuẩn bị môi trường

## Tải bài lab

```bash
cd /home/student/labtainer/labtainer-student
imodule https://github.com/qlh2404/stego-mfcc-encode/raw/refs/heads/main/imodule.tar
```

## Khởi tạo bài lab

```bash
labtainer -r stego-mfcc-encode
```

## Cài đặt thư viện

```bash
pip3 install librosa numpy scipy matplotlib soundfile
```

---

# 5. Nội dung thực hành

## Task 1: Tiền xử lý

Xem file:

```bash
nano preprocess.py
```

Chạy tiền xử lý và trích xuất MFCC:

```bash
python3 preprocess.py
```

---

## Task 2: Giấu thông điệp

Xem file encode:

```bash
nano encode.py
```

Nhập thông điệp:

```bash
nano secret.txt
```

Nhập:

```
secret message
```

Chạy giấu tin:

```bash
python3 encode.py
```

---

## Task 3: Đánh giá chất lượng

Xem file evaluate:

```bash
nano evaluate.py
```

Chạy đánh giá:

```bash
python3 evaluate.py
```

Cài đặt eog để xem ảnh:

```bash
sudo apt update
sudo apt install eog
```

Xem biểu đồ:

```bash
eog mfcc_comparison.png
```

Xem báo cáo:

```bash
cat mfcc_report.txt
```

So sánh biểu đồ âm thanh gốc và âm thanh đã giấu tin.

---

# 6. Checkwork và kết thúc bài lab

```bash
checkwork stego-mfcc-encode
stoplab stego-mfcc-encode
```

Sau khi kết thúc, file zip kết quả sẽ được tạo.

---

# 7. Khởi động lại bài lab

```bash
labtainer -r stego-mfcc-encode
```

---

# Tài liệu tham khảo

* Đ. X. Chợ, *Giấu tin trong âm thanh dùng kỹ thuật tự đánh dấu*, 2023.

---

Nếu bạn muốn README **chuẩn GitHub đẹp hơn (có ảnh, workflow, structure project)** thì mình có thể format lại chuyên nghiệp hơn nữa.
Mình đã đọc nội dung PDF của bạn , dưới đây là phiên bản **định dạng Markdown để bạn đưa thẳng vào README.md trên GitHub**.

Bạn chỉ cần copy toàn bộ phần dưới:

---

# stego-mfcc-encode

**Audio Steganography using MFCC Features**

## Giới thiệu

Bài lab thực hiện kỹ thuật giấu tin trong âm thanh sử dụng đặc trưng MFCC (Mel-Frequency Cepstral Coefficients).
Sinh viên sẽ thực hiện trích xuất MFCC, giấu thông điệp vào MFCC và đánh giá chất lượng âm thanh sau khi giấu tin.

---

# 1. Mục đích

* Hiểu và thực hành kỹ thuật giấu tin trong âm thanh sử dụng MFCC.
* Thực hành tạo thông điệp bí mật và giấu vào tín hiệu âm thanh.
* Nắm được nguyên lý steganography trong âm thanh dựa trên đặc trưng MFCC.

---

# 2. Yêu cầu

Sinh viên cần:

* Hiểu nguyên lý giấu tin trong âm thanh bằng MFCC.
* Thực hiện các bước:

  * Trích xuất MFCC
  * Giấu tin vào MFCC
  * Đánh giá kết quả bằng MSE
* So sánh sự khác biệt giữa âm thanh gốc và âm thanh đã giấu tin.

---

# 3. Kịch bản bài lab

Trong bài lab này, bạn đóng vai trò **người gửi (sender)** muốn giấu một thông điệp bí mật vào file âm thanh WAV.

## Đầu vào

* `sample.wav`

## Đầu ra

* `stego_audio.wav` – Âm thanh đã giấu tin
* `mfcc_stego.npy` – MFCC sau khi giấu tin
* `waveform_comparison.png` – Biểu đồ so sánh dạng sóng
* `waveform_report.txt` – Báo cáo MSE

---

# 4. Chuẩn bị môi trường

## Tải bài lab

```bash
cd /home/student/labtainer/labtainer-student
imodule https://github.com/qlh2404/stego-mfcc-encode/raw/refs/heads/main/imodule.tar
```

## Khởi tạo bài lab

```bash
labtainer -r stego-mfcc-encode
```

## Cài đặt thư viện

```bash
pip3 install librosa numpy scipy matplotlib soundfile
```

---

# 5. Nội dung thực hành

## Task 1: Tiền xử lý

Xem file:

```bash
nano preprocess.py
```

Chạy tiền xử lý và trích xuất MFCC:

```bash
python3 preprocess.py
```

---

## Task 2: Giấu thông điệp

Xem file encode:

```bash
nano encode.py
```

Nhập thông điệp:

```bash
nano secret.txt
```

Nhập:

```
secret message
```

Chạy giấu tin:

```bash
python3 encode.py
```

---

## Task 3: Đánh giá chất lượng

Xem file evaluate:

```bash
nano evaluate.py
```

Chạy đánh giá:

```bash
python3 evaluate.py
```

Cài đặt eog để xem ảnh:

```bash
sudo apt update
sudo apt install eog
```

Xem biểu đồ:

```bash
eog mfcc_comparison.png
```

Xem báo cáo:

```bash
cat mfcc_report.txt
```

So sánh biểu đồ âm thanh gốc và âm thanh đã giấu tin.

---

# 6. Checkwork và kết thúc bài lab

```bash
checkwork stego-mfcc-encode
stoplab stego-mfcc-encode
```

Sau khi kết thúc, file zip kết quả sẽ được tạo.

---

# 7. Khởi động lại bài lab

```bash
labtainer -r stego-mfcc-encode
```

---

# Tài liệu tham khảo

* Đ. X. Chợ, *Giấu tin trong âm thanh dùng kỹ thuật tự đánh dấu*, 2023.

---

Nếu bạn muốn README **chuẩn GitHub đẹp hơn (có ảnh, workflow, structure project)** thì mình có thể format lại chuyên nghiệp hơn nữa.
