+++
author = "koji00"
title = "Speedtest-CLI | Speedtest.net command line interface"
date = "2020-01-01"
description = "Hôm nay mình sẽ giới thiệu giao diện dòng lệnh của công cụ này speedtest-cli"
tags = [
    "tool",
    "command",
]
categories = [
    "linux",
]
aliases = ["migrate-from-thinkview"]
images  = ["img/2020/speedtest-cli.png"]
+++

Chắc hẳn mọi người đã quá quen với Speedtest.net khi muốn kiểm tra tốc độ Internet rồi nhỉ?

Hôm nay mình sẽ giới thiệu giao diện dòng lệnh của công cụ này `speedtest-cli`

## Yêu cầu:
Cần có `python` >2.4

## Cài đặt:

* với pip: `pip install speedtest-cli`
* với git:
    ```
    git clone https://github.com/sivel/speedtest-cli.git
    cd speedtest-cli
    python setup.py install
    ```
> Gợi ý: nên tìm hiểu thêm về `python`, `pip`, các lệnh với file, thư mục và `git`

## Sử dụng:

  * Xem các optional arguments: `speedtest-cli -h`
  * Sử dụng arguments bạn cần, ví dụ: `speedtest-cli --bytes --secure` (đo bằng Mbyte/s và dùng HTTPS thay cho HTTP)

> Gợi ý: nên tìm hiểu thêm về arguments khi dùng command trên linux

## Repo:
https://github.com/sivel/speedtest-cli