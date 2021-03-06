# Mục đích

Hướng dẫn thực hiện cài đặt việc copy clipboard giữa window và virtualBox

## Tải file iso

```shell
sudo apt-get install virtualbox-guest-additions-iso
```

Nếu trong quá trình cài đặt có lỗi như bên dưới

```shell
could not get lock /var/lib/dpkg/lock-frontend
```

Thì thực hiện các dãy câu lệnh như sau

```shell
sudo killall apt apt-get

sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock*

sudo dpkg --configure -a

sudo apt update
```

## Mount file iso

Sau khi tải file iso thì mount vào với ubuntu

![image](https://user-images.githubusercontent.com/28853808/76238277-30025e00-6262-11ea-80a9-7ebf232a7e4e.png)

![image](https://user-images.githubusercontent.com/28853808/76238412-67710a80-6262-11ea-83a7-50ecfee5e613.png)

Nhập mật khẩu nếu có, và chọn "Run"

## Tùy chọn copy

Thay đổi cài đặt copy

> Device > Share Clipboard > Bidirectional

![image](https://user-images.githubusercontent.com/28853808/76238580-a43d0180-6262-11ea-8f71-158c15b8058b.png)

Khởi động máy lại và tận hưởng thành quả.
