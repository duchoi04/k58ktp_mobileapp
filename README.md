MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

BÀI TẬP LỚN:

1. Viết phần mềm trên công cụ Mit App inventor

   (tập trung vào quy trình tạo ra phần mềm)
   
   app có 3 screen:
   
   + about về bản thân+nút gọi sang 2 screen còn lại
   
   + giải 1 bài toán đơn giản
   
   + sử dụng webview: hiển thị 1 trang web có sẵn, hỗ trợ giao diện điện thoại
   
   mô tả: thanh công cụ có gì? kéo thả + thay đổi thuộc tính: làm ntn, để làm gì?
   
block: mô tả bản chất việc kéo thả block ntn?

ưu điểm gì so với viết code? nhược điểm?

copy paste block ? (backpack)
   
3. Viết app sử dụng Android Studio

   + Android manifest.xml  => mô tả gì? app cần quyền để do-st: khai báo ntn? để làm gì?

   + vòng đời của 1 ứng dụng android.

     code tự sinh sau khi tạo 1 project: có sẵn hàm onCreate: tại sao???
     
   + Code: java language.

app cần check xem có quyền để do-st? : code ntn? ý nghĩa?

giao diện: (res/layout) mô tả bằng file XML + UI Design review

+ thuộc tính text, hoặc các thuộc tính khác: giá trị hardcode => lưu vào nới khác, tham chiếu tới nó:

cú pháp của việc tham chiếu là gì?
ưu điểm của việc tham chiếu này?
OS hỗ trợ auto việc lấy giá trị tham chiếu theo LOCATION, LANGUAGE, THEME
việc hỗ trợ auto này giúp app làm được điều gì?

+ đối tượng chứa: gộp các đối tượng con lại: cùng 1 quy luật sắp xếp để hiển thị

các đối tượng con nằm kề nhau theo chiều dọc | hoặc ngang, gravity

code tương tác với layout: vd hiển thị text

mong muốn text hiển thị phù hợp với thiết lập LOCATION, LANGUAGE, THEME của người dùng thì làm ntn? (tránh hardcode)

event (sự kiện) người dùng tác động vào app: CLICK vào button, click vào text,...

với 1 sự kiện nào đó, muốn chạy 1 đoạn code để do-st thì LAYTOUT cần làm gì?

CODE viết như nào (2 cách)

---------------------------
trong app có các thư mục đặc biệt: Assets
     
khi sử dụng Window Explorer để copy các files + folder vào trong Assets
     
thì khi compiler: mọi file này đều đi theo app, nằm trong app
     
trong app có thể truy cập được đến các file này
     
cú pháp truy cập vào là gì?
     
lợi ích của việc app có sẵn các files (offline cũng có)?
     
ứng dụng: app hướng dẫn việc X
   
==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets

format dữ liệu: tuỳ ý, nội dung tuỳ ý
         
công cụ để hiển thị dữ liệu: tuỳ ý
         
có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý.
         
SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ
         
MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ:

DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN)

DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU.

(ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN)      
                    
------------------------

APP2 (android studio):  tạo app tương đương với Mit App inventor

app có 3 activity
  
  + activity1: about: about+nút gọi sang 2 activity còn lại
    
  + activity2: giải toán đơn giản (tuỳ ý). mỗi khi giải xong bài toán: gọi api tại https://k58kmt.tdh.io.vn/api để gửi bài toán lên đó
    
{app_by:mã số sv, input: {a:1,b:2,c:3,name:"hello tắc kè"},output:{ketluan:"vô nghiệm", abc:"xyz", nghiem:3.14}} nhận lại json: {ok:1, stt:1234}
    
  + activity3:
dùng web-view để truy cập từ
    
1 trang web https://k58kmt.tdh.io.vn?masv=mã sv của bạn
    
=======================

vết để lại: mô tả quá trình làm bài tập ra file .md => upload github
    
kèm hình ảnh minh hoạ quá trình làm.
    
print ra giấy đóng quyển, nộp bm.
    

BÀI LÀM


BÀI 1: Viết phần mềm trên công cụ Mit App inventor

1. Khởi tạo: Truy cập trang web ai2.appinventor.mit.edu (đăng nhập bằng tài khoản Google), bấm Start new project và đặt tên dự án


<img width="1920" height="1080" alt="Screenshot 2026-06-10 155243" src="https://github.com/user-attachments/assets/d6ced0df-06ba-4753-81ad-efb04da6f521" />

2. Kéo thả linh kiện: Tại cột User Interface (Bên trái), tiến hành kéo thả các thành phần vào màn hình điện thoại ở giữa (Viewer):


Label: Để hiển thị văn bản (Họ tên: Hoàng Đức Hội, MSSV...).


Button: Nút bấm để thực hiện lệnh hoặc chuyển màn hình.


TextBox / Image: Để nhập dữ liệu hoặc hiển thị hình ảnh (nếu bài yêu cầu).


Đổi thuộc tính (Properties): Nhìn sang cột bên phải cùng để chỉnh lại kích thước chữ (FontSize), màu nền (BackgroundColor), và

căn giữa màn hình 

(AlignHorizontal chọn Center).


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1a8d9a64-d929-4ff1-9d5e-5813216d7b87" />

3. Tạo Screen1 kéo vào màn hình điện thoại 2 label, 2 Button và đổi tên theo tên của mình:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/52f626f5-a784-46ae-8402-ea62318efe76" />


4. Tạo Screen2 kéo vào 2 Label, 2 TextBox, 1 Button và đổi tên theo tên của mình:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/01e8dcda-efd7-4b0c-8ace-c04145225646" />


5. Tạo Screen3 kéo vào 1 WebViewer và dán link trang web vào phần HomeURL ở bên phải màn hình khi bấm vào WebViewer:


<img width="1920" height="1080" alt="Screenshot 2026-06-10 161343" src="https://github.com/user-attachments/assets/fac4e7cb-51a1-4b6b-92fc-f5879f554314" />


6. Sau đó bấm chuyển sang Blocks cấu hình 3 Screen:


<img width="440" height="450" alt="image" src="https://github.com/user-attachments/assets/e3ef5bdd-7153-4001-aef2-d26abd4bfd88" />



7.  Bấm vào btnToan rồi kéo when btnToan .Click ở dòng đầu tiên ra màn hình



<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b62ff3cc-51f5-45ae-91f8-4e94fec205be" />



8.  Tiếp theo bấm Control màu vàng ở phần Built-in kéo another screen ra màn hình và nối vào btnToan.click:



<img width="1649" height="994" alt="image" src="https://github.com/user-attachments/assets/f800ab36-a343-43d9-a23e-61d75bf37172" />



9.  Rồi bấm vào ô Text màu hồng kéo phần có "" ra màn hình và nối vào như hình và đổi tên thành Screen2:


<img width="1507" height="998" alt="image" src="https://github.com/user-attachments/assets/1bb6dc49-bd69-42e0-bdad-2005d6a3631d" />


10. btnWeb chỉ cần coppy btnToan past ra và đổi tên từ Screen2 thành Screen3 là được:


<img width="745" height="444" alt="image" src="https://github.com/user-attachments/assets/3bdac746-8bcb-4ed7-a34b-d2fdd4d8b590" />



11. Bấm vào Screens chuyển sang Screen2 và tiếp tục cấu hình:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f485b01b-2cab-41cc-a300-53b7679d73fd" />



12. When btnCong.click kéo ra như bước trên


Bấm vào set lblKetQua. Text to kéo ra màn hình nối vào When btnCong.click:



<img width="1815" height="939" alt="image" src="https://github.com/user-attachments/assets/2594d4f2-83ba-4785-a41c-7db107a9a112" />



13. Sau đó bấm vào các Math màu xanh dương chọn các phép toán tùy ý và nối vào như hình:


<img width="1746" height="991" alt="image" src="https://github.com/user-attachments/assets/78bf95a5-454f-49e0-aab5-8b81d9a6f8f1" />



14. Rồi bấm vào phần txtSo1 và txtSo2 kéo txtSo1.Text và txtSo2.Text ra màn hình đặt vào trong Math màu xanh dương:


<img width="1920" height="1067" alt="image" src="https://github.com/user-attachments/assets/de62c860-4a2e-40c3-8640-5b92cc797070" />

15. Chuyển sang Screen3 và cấu hình như trong hình:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/439306fa-f79b-409c-9850-b2f3e0533973" />

16. Kết nối lên điện thoại bằng cách tải app MIT APP Inventor trên CH Play hoặc App Store về sau đó ở trang Web bấm vào phần Connect trên đầu trang và bấm vào AI Companion sẽ hiện ra code và mã QR để đăng nhập:

<img width="1237" height="679" alt="image" src="https://github.com/user-attachments/assets/c9fa6006-a2c2-4bc3-aff9-3c41dbd1f817" />


<img width="1156" height="951" alt="image" src="https://github.com/user-attachments/assets/8794ebdc-103b-4fce-9c92-d77632c17ac5" />

 KẾT QỦA:

<img width="1179" height="2556" alt="image" src="https://github.com/user-attachments/assets/1887da61-8c28-436e-9b70-7d7f5491673e" />

<img width="1179" height="2556" alt="image" src="https://github.com/user-attachments/assets/08891182-1da7-46d2-947f-cf6d65a31870" />

<img width="1179" height="2556" alt="image" src="https://github.com/user-attachments/assets/82ff11a9-bc4d-46e5-8ef7-531382185264" />


BÀI 2: Viết app sử dụng Android Studio

Đề xuất triển khai App 1: "Sổ tay Chính sách Tài xế Xanh SM"

Đây là một bài toán thực tế kết hợp giải quyết vấn đề bằng Assets:


Vấn đề đặt ra: Các tài xế xe điện Xanh SM cần tra cứu nhanh các mốc tỷ lệ hoàn thành chuyến, chu kỳ xét hạng và chính sách
thưởng phạt. Tuy nhiên, khi di chuyển ở các vùng sóng 4G yếu hoặc ngoại ô, việc mở app trực tuyến thường bị xoay vòng (loading)
mất thời gian.

Cách giải quyết: Đưa toàn bộ nội dung chính sách định dạng tĩnh vào app thông qua file Assets để tra cứu Offline 100%.


Đặc thù dữ liệu: Dữ liệu dạng văn bản phân cấp, lưu trong file policy.json đặt tại thư mục Assets.


Thuật toán xử lý:


Mở luồng InputStream đọc file JSON từ Assets.


Dùng thuật toán đọc luồng byte (BufferedReader) ghép thành chuỗi String hoàn chỉnh.


Dùng thư viện org.json.JSONObject để bóc tách chuỗi String ra thành các mốc dữ liệu thưởng tương ứng.


Đối tượng hiển thị: Sử dụng thành phần RecyclerView kết hợp CardView để liệt kê các mục chính sách một cách đẹp mắt, chuyên

nghiệp.

BƯỚC 1: TẠO DỰ ÁN MỚI 

Mở Android Studio, chọn File ➔ New ➔ New Project...


Chọn mẫu Empty Views Activity (Tuyệt đối không chọn Empty Activity nhé). Nhấn Next.


Ô Name gõ: App1_Assets


Ô Language chọn: Java.


Nhấn Finish. Chờ khoảng 1-2 phút để thanh màu xanh dưới đáy màn hình chạy xong hẳn (hiện chữ Daemon started successfully).


<img width="1332" height="1067" alt="image" src="https://github.com/user-attachments/assets/56ada31d-64e4-43a0-a72e-f4eb3d3ee789" />

BƯỚC 2: CÁCH TẠO THƯ MỤC ASSETS VÀ FILE JSON

Đây là bước quan trọng nhất để nạp dữ liệu Offline. Nhìn sang cột quản lý thư mục bên trái màn hình:


Click chuột phải vào chữ app.


Trỏ chuột vào chữ New ➔ Kéo xuống dưới cùng chọn Folder ➔ Chọn Assets Folder.


<img width="938" height="1080" alt="image" src="https://github.com/user-attachments/assets/72ab1bc7-7957-4660-9349-3b84028fe817" />


Một bảng hiện ra, cứ để nguyên mặc định và bấm Finish.

<img width="1416" height="1077" alt="image" src="https://github.com/user-attachments/assets/42a6acb8-ba82-4e94-83d1-d3b40a491fb7" />


Lúc này sẽ thấy một thư mục tên là assets màu vàng xuất hiện ngang hàng với thư mục java và res.


<img width="310" height="287" alt="image" src="https://github.com/user-attachments/assets/fab4024c-d47c-478b-b4f5-b2903c9b2a0d" />


Click chuột phải vào chính thư mục assets vừa tạo đó.

Chọn New ➔ Chọn File.

<img width="889" height="1045" alt="image" src="https://github.com/user-attachments/assets/5e758ee0-0b45-4180-a4a3-ee0fcd84c368" />


Gõ tên file là: policy.json rồi nhấn Enter.


File trắng sẽ mở ra, Copy đoạn dữ liệu JSON rồi dán vào:


<img width="1920" height="833" alt="image" src="https://github.com/user-attachments/assets/3fcf9694-4092-4387-bc38-0b59931266a9" />


BƯỚC 3: CÁCH LÀM GIAO DIỆN MÀN HÌNH CHÍNH (activity_main.xml)


Ở cột bên trái, bạn mở theo đường dẫn: app ➔ res ➔ layout.


Click đúp chuột để mở file activity_main.xml.


Nhìn lên góc trên cùng bên phải của màn hình code, có 3 nút: Code | Split | Design. Bấm chọn nút Code (hoặc biểu tượng có các đường kẻ ngang) để nó hiện ra toàn chữ:

<img width="319" height="252" alt="image" src="https://github.com/user-attachments/assets/0dd5b37c-b057-479b-a516-bbb14b0668bb" />


Nhấn Ctrl + A để bôi đen tất cả code cũ sinh sẵn, bấm nút Delete để xóa sạch đi.


Copy đoạn code XML phần activity_main.xml rồi dán vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1ea9d821-f254-44ab-9dc1-a16f795cc6e0" />


BƯỚC 4: CÁCH TẠO GIAO DIỆN THẺ BÀI (item_policy.xml)

Vì danh sách có nhiều mục, ta cần làm 1 cái khuôn (thẻ bài) để nhét dữ liệu vào.


Click chuột phải vào thư mục layout (nằm trong res).


Chọn New ➔ Chọn Layout Resource File.


<img width="1077" height="1070" alt="image" src="https://github.com/user-attachments/assets/a7e266b8-07b5-4797-8334-b1fef173b031" />



Ở ô File name đầu tiên, gõ chữ: item_policy (viết thường, dùng dấu gạch dưới). Nhấn OK.


<img width="1061" height="994" alt="image" src="https://github.com/user-attachments/assets/470d5ebb-9edd-4b6b-bb79-a8ed2cfe7f42" />


File mới mở ra, lại bấm sang chế độ Code (ở góc phải trên cùng).


Xóa sạch code tự sinh, copy đoạn code XML phần item_policy.xml rồi dán vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c5f6a44f-6307-4323-84a9-87af2ada0a24" />


BƯỚC 5: CÁCH DÁN CODE JAVA 


Mở file theo đường dẫn: app ➔ java ➔ com.example.app1_assets ➔ MainActivity.java.



<img width="428" height="496" alt="image" src="https://github.com/user-attachments/assets/e63d31b4-d409-4ef6-99db-6952747eb2fe" />



Khi file mở ra, hãy nhìn vào Dòng số 1. Nó sẽ có dạng:


package com.example.app1_assets;


TUYỆT ĐỐI KHÔNG XÓA DÒNG NÀY.


Dùng chuột bôi đen toàn bộ các chữ từ dòng số 2 trở xuống đến hết, rồi bấm Delete.


Bây giờ, copy đoạn code Java (copy từ dòng số 3 trở đi - tức là bắt đầu copy từ chữ import

android.os.Bundle; xuống tận cùng). Dán phần code vừa copy đó vào dưới dòng 1:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cf016871-1ba7-404f-ab12-b1df42a69d3d" />


BƯỚC 6: CHẠY THỬ 

<img width="1920" height="1080" alt="Screenshot 2026-06-11 120345" src="https://github.com/user-attachments/assets/b97ee5ee-d61d-4ddc-9018-cfec6010c320" />

Sau khi chạy đã thấy app hiện ra 





BÀI 3: APP2 (android studio):  tạo app tương đương với Mit App inventor

BƯỚC 1: KHỞI TẠO & CẤU HÌNH HỆ THỐNG 

Thao tác: Mở Android Studio ➔ Chọn File ➔ New ➔ New Project...


Chọn cấu trúc: Tại cửa sổ chọn mẫu, bắt buộc chọn Empty Views Activity


Thiết lập thông số: * Đặt tên ứng dụng (Name): App2_Final


Ngôn ngữ (Language): Java


Minimum SDK: API 24 (Android 7.0) để đảm bảo tối ưu hiệu năng.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b7140a40-4b95-40ef-9470-275be5bce1e0" />


Sau khi nhấn Finish, đợi thanh tiến trình Gradle nạp xong toàn bộ cây thư mục cấu trúc.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e3fbed64-a2fa-43d2-b7bf-0b53e5fcbefc" />


BƯỚC 2: THIẾT KẾ MÀN HÌNH 1 - ABOUT ME

1. File Giao diện (activity_main.xml):

Mở file app -> res -> layout -> activity_main.xml, chuyển sang chế độ gõ Code (biểu tượng các đường kẻ ngang ở góc trên bên phải), xóa hết code cũ và dán code vào:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b85a7982-d315-4aea-a475-a35e1e9638ea" />

2. File Xử lý Logic (MainActivity.java):

Mở file app -> java -> com.example.app2_final -> MainActivity, xóa hết đi và dán đoạn code điều hướng chuyển màn hình này
vào:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ea4b1a34-f079-4285-a8f2-b7885aecc595" />

BƯỚC 3: TẠO VÀ CÀI ĐẶT MÀN HÌNH 2 - GIẢI TOÁN & GỌI API

Bây giờ bạn hãy tự tạo thủ công các file cho màn hình số 2 để không lo phần mềm bị treo bảng cài đặt tự động nữa nhé:


1. Tạo file Java (MathActivity.java):


Click chuột phải vào thư mục com.example.app2_final -> chọn New -> Java Class.


<img width="1920" height="1080" alt="Screenshot 2026-06-11 105204" src="https://github.com/user-attachments/assets/e9a74e41-400a-40fa-af31-b1239463175b" />


Gõ tên là: MathActivity rồi nhấn Enter.


Mở file vừa tạo ra, xóa hết chữ bên trong và dán đoạn code xử lý giải toán + đóng gói JSON + gửi API bằng luồng chạy ngầm này

vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/37b7b5ac-5003-4a50-b5bb-c2e094a56d23" />



2. Tạo file Giao diện (activity_math.xml):
   

Click chuột phải vào thư mục res -> layout -> chọn New -> Layout Resource File.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d20cd7f1-180c-4496-a695-1d47c1e314f4" />



Ô File name gõ chữ: activity_math rồi ấn OK.


Chuyển sang chế độ gõ Code, xóa hết đi và dán đoạn mã vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/09bda39a-d02e-4c33-a354-e401623eea62" />



BƯỚC 4: TẠO VÀ CÀI ĐẶT MÀN HÌNH 3 - WEBVIEW


1. Tạo file Java (WebActivity.java):


Click chuột phải vào thư mục com.example.app2_final -> chọn New -> Java Class.


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/24d8689c-2c7c-4c01-aabf-c7fc0cec4e61" />


Gõ tên là: WebActivity rồi nhấn Enter.


Mở file ra, xóa hết chữ bên trong và dán đoạn code vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f8f6387a-d4da-42c6-91ad-6d6953cf8d4f" />

2. Tạo file Giao diện (activity_web.xml):
   

Click chuột phải vào thư mục res -> layout -> chọn New -> Layout Resource File.


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e64240e6-ecd6-425d-909c-ef97a71e1e90" />


Ô File name gõ chữ: activity_web rồi ấn OK.


Chuyển sang chế độ gõ Code, xóa hết đi và dán code vào:


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/648acc7b-5ef0-45d8-aee5-baaeabd4a5e0" />


CÁC BƯỚC TẠO MÁY ẢO ĐỂ TEST APP TRÊN MÁY TÍNH


Bước 1: Mở trình quản lý thiết bị (Device Manager)


Nhìn lên thanh công cụ phía trên cùng bên phải của Android Studio.


Tìm và click vào biểu tượng Device Manager (hình một chiếc điện thoại nhỏ có sọc dọc ở góc phải, hoặc bạn có thể vào menu Tools 

Device Manager.

<img width="709" height="469" alt="image" src="https://github.com/user-attachments/assets/815d5a78-2c81-4c9e-a4e0-393c5819f375" />



Bước 2: Bắt đầu tạo mới


Ở bảng Device Manager vừa hiện ra ở mép phải màn hình, bạn bấm vào nút Create device (hoặc biểu tượng dấu cộng +):

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/73766f94-ebb2-4c2d-905c-c5193a8f9720" />


Bước 3: Chọn dòng điện thoại mô phỏng


Một cái bảng danh sách hiện ra, bạn chọn mục Phone ở cột trái.


Ở cột giữa, bạn chọn một mẫu điện thoại phổ biến và nhẹ, ví dụ: Pixel 7 hoặc Pixel 6 (chú ý chọn cái nào có biểu tượng Play

Store ở cột bên cạnh để dễ test webview nhé).


Nhấn Next.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/56e55449-5257-4a27-ab9f-cddbe0b20ef2" />


Bước 4: Chọn phiên bản hệ điều hành (System Image)


Lúc này phần mềm sẽ hỏi muốn máy ảo chạy Android mấy. Nên chọn các bản ổn định như VanillaIceCream (API 35),

UpsideDownCake (API 34) hoặc Tiramisu (API 33).


Nếu bên cạnh tên phiên bản có một mũi tên xanh chỉ xuống (Download),  hãy click vào đó để máy tính tự tải gói Android đó về

(quá trình tải mất khoảng 1-2 phút tùy mạng).


Sau khi tải xong, chọn phiên bản đó và nhấn Next.


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9bce340f-f66e-4933-b122-2adbca0ed3cf" />


Sau khi xong bấm chạy chương trình và bấm vào phần Running Devices sẽ thấy máy ảo và app vừa tạo hiện ra:

<img width="1016" height="1037" alt="image" src="https://github.com/user-attachments/assets/fa943519-bc4a-44ec-8fb1-6afacbb48cfc" />

KẾT QUẢ TEST: 

Giair toán:

<img width="773" height="1080" alt="image" src="https://github.com/user-attachments/assets/299b89fc-aad9-41d3-9e45-5d7c86ed6815" />

Mở màn hình Website:

<img width="781" height="1080" alt="image" src="https://github.com/user-attachments/assets/205d73a7-d233-4e99-ac8b-53026216fb1f" />



























































































































































