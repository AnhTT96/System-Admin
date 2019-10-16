# Hướng dẫn cấu hình và sử dụng iDRAC Server Dell

 

## Mục lục
1. Tìm hiểu về iDRAC  
2. Cài đặt iDRAC
3. Giám sát các thông tin trên iDRACDell

## 1. Tổng quan về iDRAC

Ngày nay, đối với một người kỹ sư hệ thống 24 tiếng một ngày dường như không đủ để tối ưu cho hệ thống của mình. Thực tế đã xảy ra rất nhiều trường hợp server vật lý để ở Datacenter gặp sự cố về phần cứng mà người quản trị không thể giám sát và có cảnh báo kịp thời dẫn tới có những sự cố downtime đáng tiếc, mang lại thiệt hại lớn cho cá nhân, tổ chức, doanh nghiệp. Có những công cụ nhỏ tích hợp sẵn trong dòng server Dell nhưng không hẳn kỹ sư hệ thống nào cũng biết đó là việc sử dụng chức năng iDRAC.

Đối với dòng server DELL thế hệ mới model Power Edge Server thế hệ thứ 12 của Dell thì đều có tích hợp  `iDRAC`(Integrated Dell Remote Access Controller) cung cấp tính năng để quản lý các thông số hardware của server từ xa, troubleshoot, remote thông qua một giao diện web người quản trị có thể không phải di chuyển tới server cắm màn hình cũng có thể thao tác với server của mình.

`iDRAC`  được cấu hình thông qua một port riêng, kết nối qua đường RJ45 được cấu hình các thông số về network.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac1.png)

## 2. Cài đặt iDRAC
-   Khởi động server DELL thao tác phím  `F2`  để vào  `System Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac2.png)

-   Quá trình vào chế độ  `Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac3.png)

-   Lựa chọn mục  `setup iDRAC`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac4.png)

-   Cấu hình địa chỉ IP cho port iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac5.png)

-   Setup user login vào iDRAC

Quay trở lại tab Setup chọn  `User Configuration`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac6.png)

Set password cho user root

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac7.png)

-   Confirm thay đổi và reboot lại server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac8.png)

–> Quá trình cài đặt thành công login vào iDRAC thông qua địa chỉ ip và username/pass đã cấu hình ở trên.

`[https://ip_idrac](https://ip_idrac/)`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac9.png)

Login thành công hiển thị giao diện dưới

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac10.png)

## 3.Giám sát các thông tin trên iDRAC

### 3.1. Tab serve
-   `Properties`: Cung cấp các thông tin chung về server và đường link truy cập nhanh tới các mục khác, cửa sổ console để remotr desktop, thao tác nhanh đối với server như Power ON /OFF…, thông tin về về server như BIOS, IP, Firmware OS.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac11.png)

-   `Attached Media`: Cấu hình cho phép việc đính kèm file ISO của OS lên hay không, chia sẻ file hay không.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac12.png)

-   `Log`: Hiển thị thông tin log đối với server có sắp xếp theo mức độ, time/date

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac13.png)

-   `Power / Thermal`: Hiển thị các thông tin về nguồn và nhiệt độ của server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac14.png)

-   `Virtual Console`: Thiết lập về các thông số cho việc console tới server từ xa.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac15.png)

-   `Setup`: Thiết lập thứ tự boot cho server khi khởi động

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac16.png)

### 3.2. Tab iDRAC Settings
Cung cấp thông tin về các thông số setup cho iDRAC như IP network, user…

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac17.png)

-   `Network`: Thông tin cấu hình network cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac18.png)

-   `User Authentication`: Thông tin liên quan đến setup user login iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac19.png)

-   `Update and Rollback`: Update firmware cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac20.png)

-   `Sessions`: Hiển thị phiên kết nối vào trình iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac21.png)

### 3.3. Tab Hardware

Cung cấp đầy đủ các thông tin về phần cứng của server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac22.png)

-   `Batteries`: Hiển thị trạng thái của pin main

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac23.png)

-   `Fan`: Thạng thái fan trong server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac24.png)

-   `CPU`: Trạng thái của CPU

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac25.png)

-   `Memory`: Trạng thái RAM

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac26.png)

-   `Front Panel`: Trạng thái biểu tượng phía mặt trước của server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac27.png)

-   `Network Devices`: Trạng thái và thông tin về các card mạng trên server và các card cắm thêm.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac28.png)

-   `Power Supplies`: Thông tin trạng thái về nguồn server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac29.png)

### 3.4. Tab chức năng storage

Hiển thị thông tin về storage của server.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac30.png)
