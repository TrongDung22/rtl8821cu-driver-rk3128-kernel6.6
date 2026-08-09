# RTL8821CU Wi-Fi Driver cho RK3128 TV Box

File driver Wi‑Fi (8821cu.ko) đã được biên dịch sẵn cho TV Box Rockchip RK3128 chạy Armbian / Linux với kernel 6.6.89-rk3128+.

## 1. Cài đặt nhanh trên TV Box

Mở Terminal trên TV Box và chạy lần lượt các bước sau.

### Bước 1: Tải driver về

```sh
wget https://github.com/TrongDung22/rtl8821cu-driver-rk3128-kernel6.6/raw/main/8821cu.ko -O 8821cu.ko
```

### Bước 2: Cài đặt và nạp driver

```sh
sudo cp 8821cu.ko /lib/modules/6.6.89-rk3128+/kernel/drivers/net/wireless/
sudo depmod -a
sudo modprobe 8821cu
```

### Bước 3: Kết nối Wi‑Fi

Gõ lệnh dưới đây để mở bảng chọn Wi‑Fi và nhập mật khẩu:

```sh
sudo nmtui
```

## 2. Thông số hệ thống

- SoC: Rockchip RK3128 (armhf / 32-bit)
- Kernel version: 6.6.89-rk3128+
- File cấu hình: `rk3128_linux_tvbox_defconfig`

## 3. Ghi nhận (Credits)

- Nguồn Kernel: [chieunhatnang-personal/linux-kernel-6.6-rk3128-tvbox](https://github.com/chieunhatnang-personal/linux-kernel-6.6-rk3128-tvbox)
- Nguồn Driver: [morrownr/8821cu-20210916](https://github.com/morrownr/8821cu-20210916)
