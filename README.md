# RTL8821CU Wi-Fi Driver for RK3128 TV Box (Kernel 6.6.89+)

Tệp module driver Wi-Fi Realtek RTL8821CU (`8821cu.ko`) đã được biên dịch sẵn (Cross-Compiled) cho các dòng TV Box chip Rockchip RK3128 đang chạy nhân Linux Kernel 6.6.89+.

## 🛠 Thông số môi trường biên dịch (System Specs)
- **SoC:** Rockchip RK3128 (ARM 32-bit / `armhf`)
- **Kernel Version:** `6.6.89-rk3128+`
- **Source Kernel:** [linux-kernel-6.6-rk3128-tvbox](https://github.com/chieunhatnang-personal/linux-kernel-6.6-rk3128-tvbox) (nhánh `rk3128-6.6`, config `rk3128_linux_tvbox_defconfig`)
- **Driver Source:** Realtek RTL8821CU (`morrownr/8821cu-20210916`)

---

## 🚀 Hướng dẫn cài đặt nhanh trên TV Box (Quick Install)

Mở Terminal trên TV Box và chạy lần lượt các lệnh sau:

### 1. Tải driver về TV Box
```bash
wget [https://github.com/TrongDung22/rtl8821cu-rk3128-kernel-6.6/raw/main/8821cu.ko](https://github.com/YOUR_GITHUB_USERNAME/rtl8821cu-rk3128-kernel-6.6/raw/main/8821cu.ko) -O 8821cu.ko
