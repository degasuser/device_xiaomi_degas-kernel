# Kernel Tree for Xiaomi 14T (`degas`)

![License: GPL-2.0](https://img.shields.io/badge/License-GPL%202.0-blue.svg)
![Platform: MT6897](https://img.shields.io/badge/Platform-MediaTek%20Dimensity%208300--Ultra-green.svg)
![Kernel: 6.1-GKI](https://img.shields.io/badge/Kernel-6.1%20GKI-orange.svg)

```
SPDX-FileCopyrightText: 1991 Linus Torvalds
SPDX-FileCopyrightText: 2024-2026 Xiaomi Communications Co., Ltd.
SPDX-FileCopyrightText: 2024-2026 MediaTek Inc.
SPDX-FileCopyrightText: 2024-2026 The LineageOS Project
SPDX-FileCopyrightText: 2026 degasuser <kudaskinroman5@gmail.com>
SPDX-License-Identifier: GPL-2.0-only
```

Kernel repository for the **Xiaomi 14T** (code-named **`degas`**, model `2406APNFAG`), powered by the **MediaTek Dimensity 8300-Ultra** (`MT6897`) chipset.

---

## 📌 Kernel Specifications

| Feature | Specification |
| :--- | :--- |
| **Device** | Xiaomi 14T (`degas` / `2406APNFAG`) |
| **SoC** | MediaTek Dimensity 8300-Ultra (`MT6897`) |
| **Architecture** | ARM64 (`aarch64`) - Cortex-A715 + Cortex-A510 |
| **Linux Kernel Base** | `6.1.138-android14-11` (GKI v4) |
| **Page Size** | 4096 bytes |
| **Header Version** | GKI v4 (`vendor_boot` / `boot`) |
| **DTB / DTBO** | MediaTek MT6897 DTB (`mt6897.dtb`) + Xiaomi overlay |

---

## 📂 Repository Contents

* `Image.lz4` — Compressed 64-bit ARM Linux kernel binary (GKI).
* `dtb/` — Device Tree Blobs for MediaTek MT6897 platform (`mt6897.dtb`).
* `dtbo.img` — Device Tree Blob Overlay image.
* `kernel-uapi-headers.tar.gz` — User-space API kernel headers.
* `modules/` — Loadable kernel modules (`.ko`) for MT6897 hardware (touch, display, UFS storage, sensors, audio, Wi-Fi).

---

## ⚖️ Legal & GPL-2.0 Compliance

This kernel tree is distributed under the terms of the **GNU General Public License version 2.0 (GPL-2.0)**, in strict accordance with the licensing requirements of the Linux kernel and open-source compliance standards.

Under Section 3 of the GNU General Public License v2.0, the corresponding source code for the Linux kernel and its open-source components is publicly available:

* **Upstream Linux / Android Common Kernel (ACK 6.1)**:  
  [https://android.googlesource.com/kernel/common/+/refs/heads/android14-6.1](https://android.googlesource.com/kernel/common/+/refs/heads/android14-6.1)
* **Xiaomi Official Open Source Kernel Repository (MiCode)**:  
  [https://github.com/MiCode/Xiaomi_Kernel_OpenSource](https://github.com/MiCode/Xiaomi_Kernel_OpenSource)
* **MediaTek Open Source Portal**:  
  [https://gitlab.com/mediatek](https://gitlab.com/mediatek)

### Related Repositories
* **Device Tree**: [https://github.com/degasuser/device_xiaomi_degas](https://github.com/degasuser/device_xiaomi_degas)
* **Vendor Blobs**: [https://github.com/degasuser/vendor_xiaomi_degas](https://github.com/degasuser/vendor_xiaomi_degas)
* **TWRP Recovery Tree**: [https://github.com/degasuser/device_xiaomi_degas-twrp](https://github.com/degasuser/device_xiaomi_degas-twrp)

---

## 👥 Authors & Credits

* **Linus Torvalds & Linux Kernel Developers** — Linux Kernel base.
* **Xiaomi Communications Co., Ltd.** — Device drivers, board configuration, and hardware bringup.
* **MediaTek Inc.** — MT6897 platform BSP, drivers, and SoC architecture support.
* **The LineageOS Project** — AOSP/LineageOS GKI infrastructure.
* **Maintainer**: degasuser
## Special Thanks

Special thanks to the mt6987-devs team for their contributions to MediaTek device development and the resources that helped with the Xiaomi 14T ("degas") bring-up.

Their work has been a valuable reference during the development of this project.

---

## 📄 License

This program is free software; you can redistribute it and/or modify it under the terms of the **GNU General Public License version 2.0** as published by the Free Software Foundation. See the [LICENSE](LICENSE) file for the full license text.

See [STOCK_PROVENANCE.md](STOCK_PROVENANCE.md) for the exact prebuilt source.
