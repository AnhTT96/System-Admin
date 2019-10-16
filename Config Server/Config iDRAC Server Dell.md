# Hu?ng d?n c?u hình và s? d?ng iDRAC Server Dell

 

## M?c l?c
1. Tìm hi?u v? iDRAC  
2. Cài d?t iDRAC
3. Giám sát các thông tin trên iDRACDell

## 1. T?ng quan v? iDRAC

Ngày nay, d?i v?i m?t ngu?i k? su h? th?ng 24 ti?ng m?t ngày du?ng nhu không d? d? t?i uu cho h? th?ng c?a mình. Th?c t? dã x?y ra r?t nhi?u tru?ng h?p server v?t lý d? ? Datacenter g?p s? c? v? ph?n c?ng mà ngu?i qu?n tr? không th? giám sát và có c?nh báo k?p th?i d?n t?i có nh?ng s? c? downtime dáng ti?c, mang l?i thi?t h?i l?n cho cá nhân, t? ch?c, doanh nghi?p. Có nh?ng công c? nh? tích h?p s?n trong dòng server Dell nhung không h?n k? su h? th?ng nào cung bi?t dó là vi?c s? d?ng ch?c nang iDRAC.

Ð?i v?i dòng server DELL th? h? m?i model Power Edge Server th? h? th? 12 c?a Dell thì d?u có tích h?p  `iDRAC`(Integrated Dell Remote Access Controller) cung c?p tính nang d? qu?n lý các thông s? hardware c?a server t? xa, troubleshoot, remote thông qua m?t giao di?n web ngu?i qu?n tr? có th? không ph?i di chuy?n t?i server c?m màn hình cung có th? thao tác v?i server c?a mình.

`iDRAC`  du?c c?u hình thông qua m?t port riêng, k?t n?i qua du?ng RJ45 du?c c?u hình các thông s? v? network.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac1.png)

## 2. Cài d?t iDRAC
-   Kh?i d?ng server DELL thao tác phím  `F2`  d? vào  `System Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac2.png)

-   Quá trình vào ch? d?  `Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac3.png)

-   L?a ch?n m?c  `setup iDRAC`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac4.png)

-   C?u hình d?a ch? IP cho port iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac5.png)

-   Setup user login vào iDRAC

Quay tr? l?i tab Setup ch?n  `User Configuration`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac6.png)

Set password cho user root

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac7.png)

-   Confirm thay d?i và reboot l?i server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac8.png)

–> Quá trình cài d?t thành công login vào iDRAC thông qua d?a ch? ip và username/pass dã c?u hình ? trên.

`[https://ip_idrac](https://ip_idrac/)`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac9.png)

Login thành công hi?n th? giao di?n du?i

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac10.png)

## 3.Giám sát các thông tin trên iDRAC

### 3.1. Tab serve
-   `Properties`: Cung c?p các thông tin chung v? server và du?ng link truy c?p nhanh t?i các m?c khác, c?a s? console d? remotr desktop, thao tác nhanh d?i v?i server nhu Power ON /OFF…, thông tin v? v? server nhu BIOS, IP, Firmware OS.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac11.png)

-   `Attached Media`: C?u hình cho phép vi?c dính kèm file ISO c?a OS lên hay không, chia s? file hay không.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac12.png)

-   `Log`: Hi?n th? thông tin log d?i v?i server có s?p x?p theo m?c d?, time/date

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac13.png)

-   `Power / Thermal`: Hi?n th? các thông tin v? ngu?n và nhi?t d? c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac14.png)

-   `Virtual Console`: Thi?t l?p v? các thông s? cho vi?c console t?i server t? xa.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac15.png)

-   `Setup`: Thi?t l?p th? t? boot cho server khi kh?i d?ng

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac16.png)

### 3.2. Tab iDRAC Settings
Cung c?p thông tin v? các thông s? setup cho iDRAC nhu IP network, user…

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac17.png)

-   `Network`: Thông tin c?u hình network cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac18.png)

-   `User Authentication`: Thông tin liên quan d?n setup user login iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac19.png)

-   `Update and Rollback`: Update firmware cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac20.png)

-   `Sessions`: Hi?n th? phiên k?t n?i vào trình iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac21.png)

### 3.3. Tab Hardware

Cung c?p d?y d? các thông tin v? ph?n c?ng c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac22.png)

-   `Batteries`: Hi?n th? tr?ng thái c?a pin main

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac23.png)

-   `Fan`: Th?ng thái fan trong server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac24.png)

-   `CPU`: Tr?ng thái c?a CPU

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac25.png)

-   `Memory`: Tr?ng thái RAM

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac26.png)

-   `Front Panel`: Tr?ng thái bi?u tu?ng phía m?t tru?c c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac27.png)

-   `Network Devices`: Tr?ng thái và thông tin v? các card m?ng trên server và các card c?m thêm.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac28.png)

-   `Power Supplies`: Thông tin tr?ng thái v? ngu?n server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac29.png)

### 3.4. Tab ch?c nang storage

Hi?n th? thông tin v? storage c?a server.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac30.png)
