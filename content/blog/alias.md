+++
author = "koji00"
title = "Viết tắt command trên Linux"
date = "2019-12-28"
description = "Viết tắt command trên Linux? Bạn không đọc nhầm đâu"
tags = [
    "shell",
    "command",
]
categories = [
    "linux",
]
aliases = ["migrate-from-thinkview"]
images  = ["img/2019/alias.jpg"]
+++

Viết tắt command trên Linux? Bạn không đọc nhầm đâu
Đã bao giờ thử dùng Linux chưa? Bạn thấy các câu lệnh thật dài dòng khó nhớ?

Mình sẽ hướng dẫn cách viết tắt các câu lệnh dài (hoặc ngắn nếu thích :D)

1. Đầu tiên bạn cần mở một text editor (vim/nano/vscodium/gedit/kate/emacs/v.v.) và truy cập đến file .bashrc (file cấu hình của bash, nếu dùng bash shell) hoặc .zshrc (zsh shell) trong thư mục home (chính xác là /home/username/).

    * Ví dụ: `$ nano /home/oknoodles/.zshrc`
    * Gợi ý: tìm hiểu thêm shell là gì / cấu trúc thư mục Linux (Unix)

2. Thêm dòng sau vào:

    * `alias lệnh_tắt='lệnh_gốc'`
    * Ví dụ: `alias spt='speedtest-cli --bytes --secure'`

3. Lưu lại và mở shell mới (mở terminal mới)

4. Trải nghiệm thôi <3<3

Gợi ý: Tìm hiểu thêm về bash: www.gnu.org/software/bash/manual/bash.pdf