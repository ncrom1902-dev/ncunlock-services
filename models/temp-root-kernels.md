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

## 5. Paired Quick Search Index (`Model + HyperOS + Temp Root Exploit + Kernel`)

- **Redmi K100 Pro (`athens`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.307.0.WPICNXM` | Kernel `6.12.69-android16-6-g0d80ee00f747-ab15461283-4k` | Aliases: K100 Pro athens, Redmi K100 Pro, K100ProAthens
- **Redmi K100 Pro (`athens`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPICNXM` | Kernel `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k` | Aliases: K100 Pro athens, Redmi K100 Pro, K100ProAthens
- **Redmi K100 Pro Max / POCO F9 Ultra (`songyuan`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.310.0.WGNCNXM` | Kernel `6.12.69-android16-6-g014ca48a80ee-ab15889839-4k` | Aliases: Redmi K100 Pro Max, POCO F9 Ultra, RedmiK100ProMax, PocoF9Ultra
- **Redmi K100 Pro Max / POCO F9 Ultra (`songyuan`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XGNCNXM` | Kernel `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k` | Aliases: Redmi K100 Pro Max, POCO F9 Ultra, RedmiK100ProMax, PocoF9Ultra
- **Redmi K90 Pro Max / POCO F8 Ultra (`myron`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPMCNXM` | Kernel `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | Aliases: Redmi K90 Pro Max, POCO F8 Ultra, Redmi-K90-Pro-Max
- **Xiaomi 17 (`pudding`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPCCNXM_17.0` | Kernel `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | Aliases: Xiaomi 17, Xiaomi-17
- **Xiaomi 17 Max (`byron`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.3.0.XAFCNXM` | Kernel `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | Aliases: Xiaomi 17 Max, Xiaomi17Max
- **Xiaomi 17 Pro (`pandora`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XBLCNXM_17.0` | Kernel `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | Aliases: Xiaomi 17 Pro, Xiaomi17Pro
- **Xiaomi 17 Ultra (`nezha`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPACNXM` | Kernel `6.12.69-android16-6-g43b5ab7e247d-abogki561813157-4k` | Aliases: Xiaomi 17 Ultra, Xiaomi17Ultra
- **POCO F7 / Redmi Turbo 4 Pro (`onyx`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.304.0.WOLEUXM` | Kernel `6.6.118-android15-8-ge56cf6b09cca-ab15511674-4k` | Aliases: POCO F7, Redmi Turbo 4 Pro, PocoF7, RedmiTurbo4Pro
- **Redmi K90 / POCO F8 Pro (`annibale`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPKCNXM` | Kernel `6.6.118-android15-8-g0908354dac1b-ab16143355-4k` | Aliases: Redmi K90, POCO F8 Pro, RedmiK90
- **Xiaomi 15 Pro (`haotian`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.309.0.WOBCNXM` | Kernel `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k` | Aliases: Xiaomi 15 Pro, Xiaomi15Pro
- **Xiaomi 15 Ultra (`xuanyuan`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.314.0.WOACNXM` | Kernel `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k` | Aliases: Xiaomi 15 Ultra, Xiaomi15Ultra
- **Xiaomi Pad 8 (`yupei`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.11.0.XPZCNXM` | Kernel `6.6.118-android15-8-g0908354dac1b-ab16143355-4k` | Aliases: Xiaomi Pad 8, Pad 8, XiaomiPad8
- **Xiaomi Pad 8 Pro (`piano`) HyperOS 4.0 temp root / kernel exploit** — Verified build `OS4.0.5.0.XPYCNXM` | Kernel `6.6.118-android15-8-gf72a02f47f4b-abogki551678766-4k` | Aliases: Xiaomi Pad 8 Pro, Pad 8 Pro, XiaomiPad8Pro
- **Xiaomi 14 (`houji`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.305.0.WNCMIXM` | Kernel `6.1.157-android14-11-g78a0a76cd7b7-ab15497637` | Aliases: Xiaomi 14, Xiaomi14
- **Redmi K70 Pro (`manet`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.306.0.WNMCNXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Redmi K70 Pro, RedmiK70Pro
- **Redmi K80 / POCO F7 Pro (`zorn`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.309.0.WOKCNXM` | Kernel `6.1.138-android14-11-g965475777129-mi` | Aliases: Redmi K80, POCO F7 Pro, RedmiK80
- **Redmi Note 14 Pro+ High Version (`amethyst`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.303.0.WOPTWXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Redmi Note 14 Pro+, Note 14 Pro+ High version, Note14ProPlus-HighVersion
- **Redmi Note 15 Pro+ / POCO M8 Pro 5G (`flourite`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.318.0.WPRCNXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Redmi Note 15 Pro+, Note 15 Pro Plus, fluorite, flourite
- **Redmi Turbo 3 / POCO F6 (`peridot`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.304.0.WNPMIXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Redmi Turbo 3, POCO F6, Turbo 3
- **Xiaomi 14 Pro (`shennong`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.310.0.WNBCNXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Xiaomi 14 Pro, Xiaomi 14 Pro Ti, Xiaomi14Pro
- **Xiaomi 14 Ultra (`aurora`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.305.0.WNAMIXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Xiaomi 14 Ultra, Xiaomi14Ultra
- **Xiaomi Pad 7 / POCO Pad X1 (`uke`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.305.0.WOZINXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Xiaomi Pad 7, POCO Pad X1, XiaomiPad7
- **Xiaomi Pad 7 Pro (`muyu`) HyperOS 3.0 temp root / kernel exploit** — Verified build `OS3.0.305.0.WOYEUXM` | Kernel `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | Aliases: Xiaomi Pad 7 Pro, XiaomiPad7Pro

---

## 6. Kernel Offset Exploit Catalog (`offsets.json` — 52 Builds)

Covers additional Xiaomi, Redmi, POCO (`Xiaomi 17 Pro Max [popsicle]`, `Xiaomi 15 [dada]`, `Xiaomi 17T`, `Redmi K80 Pro / K80 Ultra`, `Redmi K90 Ultra`, `Redmi Turbo 5 Max / POCO X8 Pro Max`, `Xiaomi Civi 5 Pro`, `Xiaomi MIX Fold 4 [goku]`, `Xiaomi 13T`, `Redmi Note 15 4G`), plus OnePlus, OPPO, and RedMagic kernels:

| Device / Codename | Macro | Exact Kernel Release (`uname -r`) | Exploit Route |
|---|---|---|---|
| **Redmi Note 15 Pro+** | `STRUCT_OFFSETS_6_1` | `6.1.118-android14-11-ga3b9c44908dd-ab13320413` | `offsets.json` |
| **Xiaomi 14** | `STRUCT_OFFSETS_6_1` | `6.1.118-android14-11-gca0ef6d17716-ab13624819` | `offsets.json` |
| **aurora, shennong, chenfeng, ruyi, uke, amethyst, houji, manet, peridot, muyu, flourite** | `STRUCT_OFFSETS_6_1` | `6.1.138-android14-11-g0c3d559bcd85-ab14529422` | `offsets.json` |
| **Infinix Note 50s 5G / Infinix GT 30 (X6876)** | `STRUCT_OFFSETS_6_1` | `6.1.145-android14-11-g09f1c0074ad7-ab14226177` | `offsets.json` |
| **vivo T4** | `STRUCT_OFFSETS_6_1` | `6.1.145-android14-11-g74d1702dab4d-ab14669069` | `offsets.json` |
| **Motorola Razr 50 Ultra / Motorola Razr+ 2024** | `STRUCT_OFFSETS_6_1` | `6.1.145-android14-11-geaa643a2c0ee-ab14763719` | `offsets.json` |
| **Zenfone 11 Ultra** | `STRUCT_OFFSETS_6_1` | `6.1.162-android14-11-gce140c0e5bf5-ab15450923` | `offsets.json` |
| **Redmi K90 Pro Max / POCO F8 Ultra, myron** | `STRUCT_OFFSETS_6_1` | `6.12.23-android16-5-g16e473de48a3-abogki462654244-4k` | `offsets.json` |
| **Xiaomi 17 / 17 Pro / 17 Pro Max / 17 Ultra, popsicle** | `STRUCT_OFFSETS_6_1` | `6.12.23-android16-5-g75e9b1c7ae7c-abogki463945075-4k` | `offsets.json` |
| **OPPO Find X9 / Find X9 Pro** | `STRUCT_OFFSETS_6_12` | `6.12.23-android16-5-g82efd98459a2-ab14457512-4k` | `offsets.json` |
| **OnePlus 15** | `STRUCT_OFFSETS_6_12` | `6.12.23-android16-5-ga8f88ad96df3-ab13929693-4k` | `offsets.json` |
| **OnePlus 15** | `STRUCT_OFFSETS_6_12` | `6.12.23-android16-5-gb2a876903b49-ab14541642-4k` | `offsets.json` |
| **Red Magic 11 Pro / Tablet 5 Pro** | `STRUCT_OFFSETS_6_12` | `6.12.23-android16-5-gf1bdb13583da-ab13761046-4k` | `offsets.json` |
| **REDMI Note 15 4G / POCO M6 Pro 4G** | `STRUCT_OFFSETS_6_12` | `6.12.30-android16-5-g6e872b4863d6-ab13847919-4k` | `offsets.json` |
| **Xiaomi 13T** | `STRUCT_OFFSETS_6_12` | `6.12.38-android16-5-g3c4da6410bcb-ab13872285-4k` | `offsets.json` |
| **OnePlus 15T** | `STRUCT_OFFSETS_6_12` | `6.12.38-android16-5-g844001fb8721-ab14552068-4k` | `offsets.json` |
| **Nothing Phone 3** | `STRUCT_OFFSETS_6_6` | `6.6.102-android15-8-gab8eb70a71b8-ab14350911-4k` | `offsets.json` |
| **Xiaomi 17T** | `STRUCT_OFFSETS_6_6` | `6.6.102-android15-8-gb01b41c2647c-ab15574720-4k` | `offsets.json` |
| **Xiaomi 17T** | `STRUCT_OFFSETS_6_6` | `6.6.102-android15-8-gfe76d1bc97fd-ab14689815-4k` | `offsets.json` |
| **OPPO Find N5** | `STRUCT_OFFSETS_6_6` | `6.6.118-android15-8-g2e6b9c3812c5-ab15114928-4k` | `offsets.json` |
| **REDMI K90 Ultra** | `STRUCT_OFFSETS_6_6` | `6.6.118-android15-8-g608a629fedf7-ab15154340-4k` | `offsets.json` |
| **OPPO Find X8 Ultra / OnePlus 13 / ACE 5 Pro** | `STRUCT_OFFSETS_6_6` | `6.6.118-android15-8-g93e223c276e7-abogki500782043-4k` | `offsets.json` |
| **REDMI K80 Pro / Turbo 5 Max / POCO X8 Pro Max / Xiaomi Pad 7 Ultra, piano, xuanyuan, haotian** | `STRUCT_OFFSETS_6_1` | `6.6.118-android15-8-gc44b714366cc-abogki519650608-4k` | `offsets.json` |
| **REDMI K90 Ultra / POCO F7, onyx, yupei, miro, piano** | `STRUCT_OFFSETS_6_1` | `6.6.118-android15-8-ge56cf6b09cca-ab15511674-4k` | `offsets.json` |
| **OPPO Pad 5 / OnePlus Pad 2 / OPPO Find X8s** | `STRUCT_OFFSETS_6_6` | `6.6.118-android15-8-ge58033dc8ea6-abogki498046332-4k` | `offsets.json` |
| **OPPO Find X8 / Find X8 Pro** | `STRUCT_OFFSETS_6_6` | `6.6.118-android15-8-gebdfad32d749-ab15099304-4k` | `offsets.json` |
| **Red Magic Tablet 3 Pro** | `STRUCT_OFFSETS_6_6` | `6.6.30-android15-8-g54dcbfbef792-ab12368803-4k` | `offsets.json` |
| **Xiaomi Civi 5 Pro / REDMI K90 / 4 Turbo / POCO F7, yupei** | `STRUCT_OFFSETS_6_1` | `6.6.77-android15-8-g4a507830d890-ab13636293-4k` | `offsets.json` |
| **Xiaomi 15** | `STRUCT_OFFSETS_6_6` | `6.6.77-android15-8-g63ce7556864c-ab13994517-4k` | `offsets.json` |
| **Xiaomi 15 Pro / REDMI K80 Pro / K80 Ultra** | `STRUCT_OFFSETS_6_6` | `6.6.77-android15-8-gca30f3b4bef6-abogki440974771-4k` | `offsets.json` |
| **POCO X8 Pro Max** | `STRUCT_OFFSETS_6_6` | `6.6.89-android15-8-g0889fe95bb10-ab14402178-4k` | `offsets.json` |
| **OPPO Pad 4 Pro** | `STRUCT_OFFSETS_6_6` | `6.6.89-android15-8-g096cdb6ecefc-ab14358676-4k` | `offsets.json` |
| **POCO X8 Pro** | `STRUCT_OFFSETS_6_6` | `6.6.89-android15-8-g8e4be6b47e40-ab14134548-4k` | `offsets.json` |
| **OnePlus 13** | `STRUCT_OFFSETS_6_6` | `6.6.89-android15-8-gf4dc45704e54-abogki446052083-4k` | `offsets.json` |
| **Red Magic Tablet 3 Pro / Red Magic 10 Pro / Red Magic 11 Air** | `STRUCT_OFFSETS_6_6` | `6.6.92-android15-8-g3637f4904cf5-ab13944661-4k` | `offsets.json` |
| **aurora, zorn** | `STRUCT_OFFSETS_6_1` | `6.1.138-android14-11-g965475777129-mi` | `offsets.json` |
| **songyuan, athens** | `STRUCT_OFFSETS_6_1` | `6.12.69-android16-6-g0d80ee00f747-ab15461283-4k` | `offsets.json` |
| **goku** | `STRUCT_OFFSETS_6_1` | `6.1.157-android14-11-g5655d633b31a-mi` | `offsets.json` |
| **muyu** | `STRUCT_OFFSETS_6_1` | `6.1.138-android14-11-g7b9e94e37cfa-mi` | `offsets.json` |
| **muyu** | `STRUCT_OFFSETS_6_1` | `6.1.118-android14-11-gc8d09ed78937-mi` | `offsets.json` |
| **pudding, nezha** | `STRUCT_OFFSETS_6_1` | `6.12.69-android16-6-gc8366273ff73-ab15162216-4k` | `offsets.json` |
| **mgvi_64_armv82** | `STRUCT_OFFSETS_6_1` | `6.1.138-android14-11-g51f8c580613d-ab13911623` | `offsets.json` |
| **Xiaomi 15 (dada) OS3.0.302.0.WOCCNXM** | `STRUCT_OFFSETS_6_6` | `6.6.77-android15-8-gf9a1d4bd8353-abogki440974771-4k` | `offsets.json` |
| **mgvi_64_armv82** | `` | `6.1.138-android14-11-g44bda9e8f6e9-ab13792638` | `offsets.json` |
| **Redmi K100 Pro Max / POCO F9 Ultra, songyuan** | `STRUCT_OFFSETS_6_12` | `6.12.69-android16-6-g014ca48a80ee-ab15889839-4k` | `offsets.json` |
| **myron** | `STRUCT_OFFSETS_6_1` | `6.12.23-android16-5-g5a0e85dd9db0-ab14499855-4k` | `offsets.json` |
| **Redmi K100 Pro Max (songyuan) OS4.0.5.0.XGNCNXM** | `STRUCT_OFFSETS_6_12` | `6.12.69-android16-6-g0a1dc0413ec7-ab16271006-4k` | `offsets.json` |
| **aurora** | `STRUCT_OFFSETS_6_1` | `6.1.157-android14-11-g2b8d37d00a12-mi` | `offsets.json` |
| **mgvi_64_armv82** | `STRUCT_OFFSETS_6_1` | `5.15.180-android13-8-00021-g46a5565a0982-ab13743836` | `offsets.json` |
| **mgvi_64_armv82** | `STRUCT_OFFSETS_6_1` | `5.15.194-android13-8-00038-g853eb7b6b965-ab15936612` | `offsets.json` |
| **houji** | `STRUCT_OFFSETS_6_1` | `6.1.157-android14-11-g78a0a76cd7b7-ab15497637` | `offsets.json` |
| **Generic / Multi-device** | `STRUCT_OFFSETS_6_1` | `6.12.38-android16-5-g1d46253471dd-ab15048002-4k` | `offsets.json` |

---

## Contact & Canonical Service Pages
- **Temp Root Service & Booking:** https://ncunlock.com/xiaomi-temp-root-remote-service/
- **NCUnlock Tool Box (Xiaomi Unlock Tool):** https://ncunlock.com/xiaomi-unlock-tool/
- **All Supported Models:** https://ncunlock.com/services/
- **Telegram Support:** https://t.me/ncunlock_own · Group: https://t.me/xiaomi_vn
- **WhatsApp Admin:** https://wa.me/84389013366 (+84 389 013 366)
