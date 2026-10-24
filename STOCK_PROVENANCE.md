# Stock prebuilt provenance

Source: Xiaomi 14T (degas), HyperOS OS3.0.303.0.WNERUXM fastboot ROM.

Archive: `degas_ru_global_images_OS3.0.303.0.WNERUXM_20260811.0000.00_16.0_ru_ccf2257d38.tgz`.

`Image.lz4` is the kernel payload of `boot.img`; `dtb/mt6897.dtb` is the DTB payload of `vendor_boot.img`; `dtbo.img` is copied from the archive. Modules and load lists come from vendor ramdisk and the stock DLKM partitions. The existing UAPI header archive is retained as a build input; it is not extracted from this ROM.

The GKI kernel release is `6.1.138-android14-11-g44bda9e8f6e9-ab13792638`. Vendor module release strings may carry the vendor build suffix; validate symbol CRCs rather than comparing the full GKI/vendor suffix.
