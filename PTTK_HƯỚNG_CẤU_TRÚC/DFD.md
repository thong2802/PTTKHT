# Mô hình luồng dữ liệu Data flow Diagram (DFD)

## 1. Khái niệm
   *  DFD luận lý(logic) diễn tả hệ thống làm gì mà không diễn tả điều đó làm như thế nào, tập trung vào các hoạt động của doanh nghiệp mà không tập trung vào hệ thống sẽ tạo dựng ra sao.
   *  DFD vật lý (physical) diễn tả hệ thống sẽ được thực hiện như thế nào, trong đó đề cập đến phần cứng, phần mềm, tập tin và con người.
## 2. Các tha thành phần.
   + Gồm 4 thành phần 
    
   + 1) Quy trình xử lí (process)
   + 2) Dòng dữ liệu (data Flow)
   + 3) Kho dữ liêu (data store)
   + 4) Các thực thể ngoài (external entity)

## 3. Các quy tắc thiết kế DFD
    + Mô hình hoá quy trình xử lí công việc trong HT bằng lược đồ DFD sẽ được thực hiện qua các bước : 
    + 1. Vẽ lược đồ ngữ cảnh
    + 2. Vẽ lược đồ DFD mức 0, 1, 2, 3....
+ Về lược đồ ngữ cảnh 
 
        + Xem HT là một quy trình tổng quát. 
        + Quy trình tông quát này được đánh giá ở mức 0. 
        + Lược đồ chỉ có quy trình xử lí, các thực thể ngoài và luồng dữ liệu, không có mô tả các nơi lưu trữ dữ liệu. 
        + Các thực thể ngoài cung cấp thông tin cho HT hoạt đồng, và tiêu thụ thông tin do HT tạo ra. 

+ Về lược đồ ở mức 0 ....

       + Được xem như là kết quả bung ra từ quy trình tổng quát số 0 của lược đồ bối cảnh . 
       + Chứa các quy trình xử lí chính của HT, các quy trình được đánh dấu mức 1.0, 2.0, 3.0 ....
       + Việc đánh số chỉ là phân biệt các quy trình chứ không thể thực hiện thứ tự của các quy trình. 
       + Ngoài thực thể ngoài, luồng dữ liệu, quy trình thì còn có thêm nơi lưu trữ dữ liệu .

+ Nguyên tắc phân mức

       + Lựơc đồ DFD mức 0 chứa tất cả các quy trình là các thành phần trong lược đồ bối cảnh .
       + Lược đồ DFD mức 1 chứa tất cả các quy trình là các thành phần trong lược đồ mức 0.
       + Quy tắc đánh số khi phân mức 
             +   Lươc đồ Bối cảnh : Quy trình 0. 
             +   LĐ MỨC 0 : 1, 2 , 3 ....
             +   LĐ mức 1 : 1.1, 1.1, 1.3 ...

## 4 Các quy tắc vẽ DFD
      
      + Mọi quy trình đều có dong dư liệu vào (input) và ra (output)
      + Đặt tên quy trình là Động tù. 
      + Tất cả các dòng dữ liệu đi đến hoặc đi từ nơi lưu trữ đều phải đi qua một quy trình. 
      + Đặt tên dòng dư liệu là Danh từ
      + Không có dòng dữ liệu nào mà di chuyển trực tiếp giữa các thực thể mà không qua quy trình nào . 
      + Mọi tương tác giữa các thực thể ngoài mà không dính líu tới quy trình nào thì không cần biểu diễn , coi như nằm ngoài hệ thống . 
      + Đặt tên các thực thể ngoài là Danh từ 
      + Dòng dữ liệu 2 chiều phải được tách ra thành 2 dòng.
      + Dòng dữ liệu tách ra tù dòng khác phải đảm bảo cùng tên . 
      + Dòng dữ liệu nhập chung vào dòng khác phải cùng tên
      + Không có dòng dữ liệu đệ quy
      + Có thể tách các mục tin trong dòng dữ liệu khi phân mức để di vào các quy trình con khác nhau.git