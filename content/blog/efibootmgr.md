+++
author = "koji00"
title = "efibootmgr - Trình quản lí UEFI BOOT ENTRY trên Linux"
date = "2020-03-05"
description = "efibootmgr có thể được sử dụng cực dễ chỉ bằng vài dòng lệnh"
tags = [
    "efibootmgr",
    "uefi",
    "boot",
]
categories = [
    "linux",
]
aliases = ["migrate-from-thinkview"]
images  = ["img/2020/efibootmgr1.jpg"]
+++

`efibootmgr` có thể được sử dụng cực dễ chỉ bằng vài dòng lệnh

## Repo:
https://github.com/rhboot/efibootmgr

## Cách sử dụng:

1. **Tất nhiên là phải cài đặt rồi (nếu chưa có sẵn):**
   * Ví dụ trên Arch based: `pacman -S efibootmgr`

2. **Xem manual nào:**
   * `efibootmgr -h`
    ![efibootmgr](/img/2020/efibootmgr2.jpg)

   * hoặc chi tiết hơn: `man efibootmgr`

3. **Xem thông tin chi tiết:**
    `efibootmgr -v`

4. **Thêm entry:**
     * `sudo efibootmgr -c -d <disk> -p <partition number> -L "tên" -l 'đường dẫn đến .efi'`
     * ví dụ phân vùng EFI là /dev/sdb1:
     `sudo efibootmgr -c -d /dev/sdb -p 1 -L "rEFInd" -l '\EFI\refind\refind_x64.efi'`
     * Lưu ý dùng `\` thay cho `/` trong phần đường dẫn.

5. **Xóa entry:**
     * `sudo efibootmgr -b <số của entry> -B`
     * ví dụ cần xóa Boot0002*:
     `sudo efibootmgr -b 2 -B`

6. **Thay đổi thứ tự boot:**
     ví dụ thứ tự hiện tại là 0001,0002,0003, bạn muốn đổi thành 0003,0001,0002: `sudo efibootmgr -o 3,1,2`

7. **Một số chức năng khác mọi người tìm hiểu thêm nhé!**
