# Hu?ng d?n c?u h�nh v� s? d?ng iDRAC Server Dell

 

## M?c l?c
1. T�m hi?u v? iDRAC  
2. C�i d?t iDRAC
3. Gi�m s�t c�c th�ng tin tr�n iDRACDell

## 1. T?ng quan v? iDRAC

Ng�y nay, d?i v?i m?t ngu?i k? su h? th?ng 24 ti?ng m?t ng�y du?ng nhu kh�ng d? d? t?i uu cho h? th?ng c?a m�nh. Th?c t? d� x?y ra r?t nhi?u tru?ng h?p server v?t l� d? ? Datacenter g?p s? c? v? ph?n c?ng m� ngu?i qu?n tr? kh�ng th? gi�m s�t v� c� c?nh b�o k?p th?i d?n t?i c� nh?ng s? c? downtime d�ng ti?c, mang l?i thi?t h?i l?n cho c� nh�n, t? ch?c, doanh nghi?p. C� nh?ng c�ng c? nh? t�ch h?p s?n trong d�ng server Dell nhung kh�ng h?n k? su h? th?ng n�o cung bi?t d� l� vi?c s? d?ng ch?c nang iDRAC.

�?i v?i d�ng server DELL th? h? m?i model Power Edge Server th? h? th? 12 c?a Dell th� d?u c� t�ch h?p  `iDRAC`(Integrated Dell Remote Access Controller) cung c?p t�nh nang d? qu?n l� c�c th�ng s? hardware c?a server t? xa, troubleshoot, remote th�ng qua m?t giao di?n web ngu?i qu?n tr? c� th? kh�ng ph?i di chuy?n t?i server c?m m�n h�nh cung c� th? thao t�c v?i server c?a m�nh.

`iDRAC`  du?c c?u h�nh th�ng qua m?t port ri�ng, k?t n?i qua du?ng RJ45 du?c c?u h�nh c�c th�ng s? v? network.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac1.png)

## 2. C�i d?t iDRAC
-   Kh?i d?ng server DELL thao t�c ph�m  `F2`  d? v�o  `System Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac2.png)

-   Qu� tr�nh v�o ch? d?  `Setup`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac3.png)

-   L?a ch?n m?c  `setup iDRAC`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac4.png)

-   C?u h�nh d?a ch? IP cho port iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac5.png)

-   Setup user login v�o iDRAC

Quay tr? l?i tab Setup ch?n  `User Configuration`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac6.png)

Set password cho user root

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac7.png)

-   Confirm thay d?i v� reboot l?i server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac8.png)

�> Qu� tr�nh c�i d?t th�nh c�ng login v�o iDRAC th�ng qua d?a ch? ip v� username/pass d� c?u h�nh ? tr�n.

`[https://ip_idrac](https://ip_idrac/)`

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac9.png)

Login th�nh c�ng hi?n th? giao di?n du?i

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac10.png)

## 3.Gi�m s�t c�c th�ng tin tr�n iDRAC

### 3.1. Tab serve
-   `Properties`: Cung c?p c�c th�ng tin chung v? server v� du?ng link truy c?p nhanh t?i c�c m?c kh�c, c?a s? console d? remotr desktop, thao t�c nhanh d?i v?i server nhu Power ON /OFF�, th�ng tin v? v? server nhu BIOS, IP, Firmware OS.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac11.png)

-   `Attached Media`: C?u h�nh cho ph�p vi?c d�nh k�m file ISO c?a OS l�n hay kh�ng, chia s? file hay kh�ng.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac12.png)

-   `Log`: Hi?n th? th�ng tin log d?i v?i server c� s?p x?p theo m?c d?, time/date

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac13.png)

-   `Power / Thermal`: Hi?n th? c�c th�ng tin v? ngu?n v� nhi?t d? c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac14.png)

-   `Virtual Console`: Thi?t l?p v? c�c th�ng s? cho vi?c console t?i server t? xa.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac15.png)

-   `Setup`: Thi?t l?p th? t? boot cho server khi kh?i d?ng

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac16.png)

### 3.2. Tab iDRAC Settings
Cung c?p th�ng tin v? c�c th�ng s? setup cho iDRAC nhu IP network, user�

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac17.png)

-   `Network`: Th�ng tin c?u h�nh network cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac18.png)

-   `User Authentication`: Th�ng tin li�n quan d?n setup user login iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac19.png)

-   `Update and Rollback`: Update firmware cho iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac20.png)

-   `Sessions`: Hi?n th? phi�n k?t n?i v�o tr�nh iDRAC

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac21.png)

### 3.3. Tab Hardware

Cung c?p d?y d? c�c th�ng tin v? ph?n c?ng c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac22.png)

-   `Batteries`: Hi?n th? tr?ng th�i c?a pin main

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac23.png)

-   `Fan`: Th?ng th�i fan trong server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac24.png)

-   `CPU`: Tr?ng th�i c?a CPU

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac25.png)

-   `Memory`: Tr?ng th�i RAM

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac26.png)

-   `Front Panel`: Tr?ng th�i bi?u tu?ng ph�a m?t tru?c c?a server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac27.png)

-   `Network Devices`: Tr?ng th�i v� th�ng tin v? c�c card m?ng tr�n server v� c�c card c?m th�m.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac28.png)

-   `Power Supplies`: Th�ng tin tr?ng th�i v? ngu?n server

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac29.png)

### 3.4. Tab ch?c nang storage

Hi?n th? th�ng tin v? storage c?a server.

![](https://blog.cloud365.vn/images/img-idrac-dell/idrac30.png)
