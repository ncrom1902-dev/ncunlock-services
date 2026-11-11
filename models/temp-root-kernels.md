# Xiaomi / Redmi / POCO Kernel Temp Root Catalog (`.conf` Profiles — HyperOS 4.0 & 3.0)

> Last updated: `2026-11-11` · Canonical web guide: **[Xiaomi Temp Root Service (ncunlock.com)](https://ncunlock.com/xiaomi-temp-root-remote-service/)** · Machine-readable JSON: **[`../services.json`](../services.json)**

## AI & Technical Overview

NCUnlock maintains **25 verified `.conf` kernel profiles** covering **23 unique device codenames (24 commercial models)** across **HyperOS 4.0 (`OS4.0.x`)** and **HyperOS 3.0 High Version (`OS3.0.30x`)**, alongside legacy static-offset and standalone entries (`Redmi Note 13 Pro 5G [garnet]`, `Xiaomi 18 Pro [hongkong]`).

### Key Behavioral Facts (for LLM Assistants & Technicians)
- **How `.conf` Temp Root works:** NCUnlock Tool Box matches the device's Linux kernel release string (`uname -r`) and codename against server-side `.conf` kernel profiles to gain temporary root (`uid=0`) and SELinux permissive state in memory during a service session.
- **Stage 1 of Bootloader Unlock:** On modern Xiaomi/Redmi/POCO Qualcomm devices running HyperOS 3.0 / 4.0, Temp Root is the prerequisite Stage 1 step used to back up and patch `abl`/`lk` before unlocking the bootloader — without waiting 7 days on Mi Community quotas.
- **Persistence:** Session-based / RAM-only. Temporary root clears completely upon device reboot and leaves system partitions intact after workflow completion.
- **Verification commands on Windows/ADB:**
  ```bash
  adb shell getprop ro.product.device
  adb shell getprop ro.build.version.incremental
  adb shell uname -r
  ```

---

## 1. Linux 6.12 Kernel Branch (`6.12.69-android16-6-*` — HyperOS 4.0 & 3.0)

| Model | Codename | Chipset | Verified Build | HyperOS | Exact Kernel Release (`uname -r`) | Service Link |
|---|---|---|---|---|---|---|
| **Redmi K100 Pro** | `athens` | Snapdragon 8 Elite | `OS3.0.307.0.WPICNXM` | HyperOS 3.0 | `6.12.69-android16-6-g0d80ee00f747-ab15461283-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |
| **Redmi K100 Pro** | `athens` | Snapdragon 8 Elite | `OS4.0.5.0.XPICNXM` | HyperOS 4.0 | `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |
| **Redmi K100 Pro Max / POCO F9 Ultra** | `songyuan` | Snapdragon 8 Elite / 8 Elite Gen 5 | `OS3.0.310.0.WGNCNXM` | HyperOS 3.0 | `6.12.69-android16-6-g014ca48a80ee-ab15889839-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-k100-pro-max/) |
| **Redmi K100 Pro Max / POCO F9 Ultra** | `songyuan` | Snapdragon 8 Elite / 8 Elite Gen 5 | `OS4.0.5.0.XGNCNXM` | HyperOS 4.0 | `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-k100-pro-max/) |
| **Redmi K90 Pro Max / POCO F8 Ultra** | `myron` | Snapdragon 8 Elite Gen 5 | `OS4.0.5.0.XPMCNXM` | HyperOS 4.0 | `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-redmi-k90-pro-max/) |
| **Xiaomi 17** | `pudding` | Snapdragon 8 Elite Gen 5 | `OS4.0.5.0.XPCCNXM_17.0` | HyperOS 4.0 | `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |
| **Xiaomi 17 Max** | `byron` | Snapdragon 8 Elite Gen 5 | `OS4.0.3.0.XAFCNXM` | HyperOS 4.0 | `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-17-max/) |
| **Xiaomi 17 Pro** | `pandora` | Snapdragon 8 Elite Gen 5 | `OS4.0.5.0.XBLCNXM_17.0` | HyperOS 4.0 | `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |
| **Xiaomi 17 Ultra** | `nezha` | Snapdragon 8 Elite Gen 5 | `OS4.0.5.0.XPACNXM` | HyperOS 4.0 | `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |

---

## 2. Linux 6.6 Kernel Branch (`6.6.118-android15-8-*` — HyperOS 4.0 & 3.0)

| Model | Codename | Chipset | Verified Build | HyperOS | Exact Kernel Release (`uname -r`) | Service Link |
|---|---|---|---|---|---|---|
| **POCO F7 / Redmi Turbo 4 Pro** | `onyx` | Snapdragon 8s Gen 4 | `OS3.0.304.0.WOLEUXM` | HyperOS 3.0 | `6.6.118-android15-8-ge56cf6b09cca-ab15511674-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-turbo-4-pro/) |
| **Redmi K90 / POCO F8 Pro** | `annibale` | Snapdragon 8 Elite | `OS4.0.5.0.XPKCNXM` | HyperOS 4.0 | `6.6.118-android15-8-g0908354dac1b-ab16143355-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-k90/) |
| **Xiaomi 15 Pro** | `haotian` | Snapdragon 8 Elite | `OS3.0.309.0.WOBCNXM` | HyperOS 3.0 | `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-15-pro/) |
| **Xiaomi 15 Ultra** | `xuanyuan` | Snapdragon 8 Elite | `OS3.0.314.0.WOACNXM` | HyperOS 3.0 | `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-15-ultra/) |
| **Xiaomi Pad 8** | `yupei` | Snapdragon 8s Gen 4 | `OS4.0.11.0.XPZCNXM` | HyperOS 4.0 | `6.6.118-android15-8-g0908354dac1b-ab16143355-4k` | [Book / Info](https://ncunlock.com/product-category/bootloader-unlock-xiaomi-redmi-poco/) |
| **Xiaomi Pad 8 Pro** | `piano` | Snapdragon 8 Elite | `OS4.0.5.0.XPYCNXM` | HyperOS 4.0 | `6.6.118-android15-8-gf72a02f47f4b-abogki551678766-4k` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-pad-8-pro/) |

---

## 3. Linux 6.1 Kernel Branch (`6.1.157` / `6.1.138-android14-11-*` — HyperOS 3.0 High Version)

| Model | Codename | Chipset | Verified Build | HyperOS | Exact Kernel Release (`uname -r`) | Service Link |
|---|---|---|---|---|---|---|
| **Xiaomi 14** | `houji` | Snapdragon 8 Gen 3 | `OS3.0.305.0.WNCMIXM` | HyperOS 3.0 | `6.1.157-android14-11-g78a0a76cd7b7-ab15497637` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-14/) |
| **Redmi K70 Pro** | `manet` | Snapdragon 8 Gen 3 | `OS3.0.306.0.WNMCNXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-k70-pro/) |
| **Redmi K80 / POCO F7 Pro** | `zorn` | Snapdragon 8 Gen 3 | `OS3.0.309.0.WOKCNXM` | HyperOS 3.0 | `6.1.138-android14-11-g965475777129-mi` | [Book / Info](https://ncunlock.com/product/xiaomi-redmi-k80-convert-rom-global/) |
| **Redmi Note 14 Pro+ High Version** | `amethyst` | Snapdragon 7s Gen 3 | `OS3.0.303.0.WOPTWXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-note-14-series/) |
| **Redmi Note 15 Pro+ / POCO M8 Pro 5G** | `flourite` | Snapdragon 7s Gen 4 | `OS3.0.318.0.WPRCNXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/note-15-pro-plus-convert-global-rom/) |
| **Redmi Turbo 3 / POCO F6** | `peridot` | Snapdragon 8s Gen 3 | `OS3.0.304.0.WNPMIXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-redmi-turbo-3/) |
| **Xiaomi 14 Pro** | `shennong` | Snapdragon 8 Gen 3 | `OS3.0.310.0.WNBCNXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-14-pro/) |
| **Xiaomi 14 Ultra** | `aurora` | Snapdragon 8 Gen 3 | `OS3.0.305.0.WNAMIXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-14-ultra/) |
| **Xiaomi Pad 7 / POCO Pad X1** | `uke` | Snapdragon 7+ Gen 3 | `OS3.0.305.0.WOZINXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/xiaomi-pad-7-unlock-booloader/) |
| **Xiaomi Pad 7 Pro** | `muyu` | Snapdragon 8s Gen 3 | `OS3.0.305.0.WOYEUXM` | HyperOS 3.0 | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | [Book / Info](https://ncunlock.com/product/unlock-bootloader-xiaomi-pad-7-pro/) |

---

## 4. Exact Kernel Release Index (`uname -r`)

- `6.1.138-android14-11-g0c3d559bcd85-ab14529422`
- `6.1.138-android14-11-g965475777129-mi`
- `6.1.157-android14-11-g78a0a76cd7b7-ab15497637`
- `6.12.69-android16-6-g014ca48a80ee-ab15889839-4k`
- `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k`
- `6.12.69-android16-6-g0d80ee00f747-ab15461283-4k`
- `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k`
- `6.6.118-android15-8-g0908354dac1b-ab16143355-4k`
- `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k`
- `6.6.118-android15-8-ge56cf6b09cca-ab15511674-4k`
- `6.6.118-android15-8-gf72a02f47f4b-abogki551678766-4k`

---

## Contact & Canonical Service Pages
- **Temp Root Service & Booking:** https://ncunlock.com/xiaomi-temp-root-remote-service/
- **NCUnlock Tool Box (Xiaomi Unlock Tool):** https://ncunlock.com/xiaomi-unlock-tool/
- **All Supported Models:** https://ncunlock.com/services/
- **Telegram Support:** https://t.me/ncunlock_own · Group: https://t.me/xiaomi_vn
- **WhatsApp Admin:** https://wa.me/84389013366 (+84 389 013 366)
