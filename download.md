![Hello][logo]

Xin chào, đây là một guide cơ bản dành cho các bạn mới tập tành làm quen với **Hackintosh**.
Vì guide này mới được thực hiện và mình chưa có nhiều kinh nghiệm nên còn nhiều thiếu sót, nếu có phần nào chưa chính xác hoặc cần chỉnh sửa, mình rất chào đón các **Pull Requests** của các bạn :smile:.

# Khởi động

Trước tiên, bạn nên biết đây là một công việc khó khăn cũng như đầy gian lao. Vì vậy hãy chuẩn bị một sự kiên nhẫn, và trong lúc đó các bạn có thể tải về các công cụ bên dưới đây.

## Tài nguyên

### Bộ cài Mac OS

Không thể thiếu, đó là các bộ cài Mac OS X, bạn có thể tải về nó từ Mac OS Appstore, tuy nhiên nó yêu cầu bạn phải có một máy Mac và tài khoản Apple (AppleID). Nếu cảm thấy nó quá rắc rối, bạn có thể tải về từ đây:

* [(Fshare) Macintosh.VN][osx-installer-macintoshvn] - mật khẩu thường là *macintosh.vn*.
* [(Fshare) appdl.store/YourApple.vn][osx-installer-yourapple] - quá nhiều quảng cáo, nhưng đành chịu thôi :rolf:.

> *Tips:* Lấy link siêu tốc fshare tại [đây](https://getlinkfshare.com).

## Công cụ thiết yếu

### Chuẩn bị đồ nghề

Vũ khí của chúng ta không gì khác chính là những chiếc USB, chuẩn USB 2.0 sẽ vận hành tốt hơn dù chậm hơn. Và dĩ nhiên nếu bạn có SSD/HDD chạy qua cổng USB sẽ không phải là một lựa chọn tồi.
Với nhu cầu của mình, sẽ có hai chiếc bao gồm:

- Một chiếc USB size khoảng **8GB** hoặc nhiều hơn:
  + **Layout**: Cần có layout GPT. Nếu USB của bạn là MBR có thể convert sang GPT hoặc xóa toàn bộ và khởi tạo layout dưới dạng GPT.
  + **Phân vùng EFI**: Clover sẽ được cài đặt vào đây và chúng ta sẽ dùng nó để boot các bộ cài. Khuyến khích các bạn lưu một bản sao các [Config][1] của Rehabman ở đây.
  + **H8H**: Phân vùng chứa các công cụ hỗ trợ cho cài đặt hackintosh.
- A large USB Flash (at least 32GB), used to accomodate all Mac OS Installer and pre installation utility. And it must satifies following criteria:
  + GPT formated partition layout with capability of booting from UEFI.
  + EFI Partition *(Min 500MiB)*: GRUB2 Installed with boot config: **Slax/PartedMagic**, **Clover > OSX PE**. Slax/Parted magic should be installed here.
  + [OS X PE](https://www.firewolf.science/firewolf-os-x-pe-v7/download-firewolf-os-x-pe-v7/)
  + Each partition for each Mac OS X Installer.

### Assets downloads

- Kexts
- Apps
- Others
- *Optional* Essential apps


[logo]: https://i.imgur.com/Ckjf5T5.png
[osx-installer-macintoshvn]: http://macintosh.vn/fshare-tong-hop-link-download-bo-cai-tat-ca-cac-phien-ban-tu-10-8-den-10-13.t109901.html
[osx-installer-yourapple]: https://appdl.store/c/macos.5/
[1]: https://github.com/RehabMan/OS-X-Clover-Laptop-Config
