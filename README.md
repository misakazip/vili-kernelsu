# Vili KernelSU Next Build

🚀 **Android kernel build with KernelSU integration for Xiaomi 11T Pro (vili)**

## 📱 Device Support

- **Device**: Xiaomi 11T Pro (vili)
- **SoC**: Snapdragon 888 (SM8350)
- **Android**: 15.0.0
- **Security Patch**: 2025-06

## ✨ Features

- 🔓 **KernelSU Next Integration**: Root access management
- 🛠️ **LineageOS Toolchain**: Clang + GCC toolchain
- 🏗️ **Automated Build**: GitHub Actions CI/CD
- 📦 **Multiple Outputs**: AnyKernel3 zip, boot.img, kernel Image

## 🚀 Usage

### Automated Build (Recommended)

1. Clone this repository.
2. Go to "Actions" tab in this repository
3. Select "Android Kernel Build (vili sm8350)" workflow
4. Click "Run workflow" and choose KernelSU option
5. Download artifacts after build completion

### Installation

#### Method 1: AnyKernel3 (Recommended)

1. Boot into custom recovery (TWRP/OrangeFox)
2. Flash `vili-kernel-kernelsu-YYYYMMDD-HHMM.zip`
3. Reboot

#### Method 2: Fastboot

```bash
fastboot flash boot boot-vili-YYYYMMDD-HHMM.img
fastboot reboot
```

## 🔒 KernelSU Next

KernelSU provides kernel-level root access management with:

- Enhanced security compared to app-level root
- Per-app permission control
- Survives system updates
- Dedicated KernelSU Manager app

## 🛠️ Build Configuration

- **Kernel Source**: [android_kernel_xiaomi_sm8350](https://github.com/sm8350-vili/android_kernel_xiaomi_sm8350.git) (branch: `15.2-ksu`)
- **Toolchain**: LineageOS Clang + GCC

## ⚠️ Disclaimer

- **Risk**: Kernel modifications can damage your device
- **No Warranty**: This software is provided as-is
- **Backup**: Always backup your original boot image
- **Self-Responsibility**: Use at your own risk

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Built with ❤️ by [misakazip](https://github.com/misakazip)
