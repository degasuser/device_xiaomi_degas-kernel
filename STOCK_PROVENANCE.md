# Stock prebuilt provenance

Source: Xiaomi 14T (degas), HyperOS OS3.0.306.0.WNEEUXM (EEA) full OTA package.

Archive: `degas_eea_global-ota_full-OS3.0.306.0.WNEEUXM-user-16.0-9185f22dfe.zip` (MD5 `9185f22dfe383ecbc438ba1075935e35`), images extracted from `payload.bin`.

`Image.lz4` is the kernel payload of `boot.img`; `dtb/mt6897.dtb` is the DTB payload of `vendor_boot.img`; `dtbo.img` is the `dtbo` image from the payload. Modules and load lists come from vendor ramdisk and the stock DLKM partitions. The existing UAPI header archive (from 6.1.138) is retained as a build input; it is not extracted from this ROM.

The GKI kernel release is `6.1.157-android14-11-g78a0a76cd7b7-ab15497637`. Vendor module release strings may carry the vendor build suffix; validate symbol CRCs rather than comparing the full GKI/vendor suffix.
