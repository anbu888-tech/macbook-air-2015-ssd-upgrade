# MacBook Air 13" Early 2015 (A1466) Complete Upgrade Guide

Comprehensive documentation for upgrading and extending the life of a **MacBook Air 13" Early 2015 (Model A1466 / MacBookAir7,2)**. Covers SSD, logic board (i5→i7), battery, thermal paste, OpenCore Legacy Patcher, and more.

---

## Machine Specs

| Spec | Detail |
|------|--------|
| Model | MacBook Air 13" Early 2015 (A1466) |
| Identifier | MacBookAir7,2 |
| RAM | 8GB LPDDR3 — **soldered, not upgradeable** |
| SSD Slot | Proprietary Apple PCIe (runs at PCIe 2.0 x4 — max ~2,000 MB/s) |
| Original SSD | Apple OEM blade SSD (proprietary connector) |

> **Key constraint:** Any modern NVMe SSD will be bottlenecked by the PCIe 2.0 x4 interface. Paying more for a high-end drive gives zero extra speed. A budget NVMe or original Apple SSD performs identically.

---

## Upgrade Options

### Option A: Original Apple SSD (No Adapter Needed)

Direct drop-in replacement from [SparesOnly.in](https://www.sparesonly.in) — [Product Page](https://www.sparesonly.in/products/macbook-air-13-a1466-early-2015-2016-2017-128gb-256gb-512gb-ssd)

- **128GB:** ₹4,720 (incl. taxes)
- **256GB:** price varies
- **512GB:** ₹8,850 (incl. taxes)
- **Warranty:** 1 year replacement
- **No adapter required**
- Original Apple SSDs from donor machines — tested and working

### Option C: Used NVMe SSD + Adapter ([Computify.in](https://computify.in))

Used/refurbished SSDs from [Computify.in](https://computify.in/collections/buy-used-ssd) (SSD collection)

| SSD | Capacity | Price | Adapter Needed | Total |
|-----|----------|-------|----------------|-------|
| [Crucial P1 500GB NVMe](https://computify.in/products/crucial-p1-500gb-pcie-3-0-3d-nand-nvme-m-2-used-ssd) | 500GB | ₹5,699 | + ₹1,584 | ~₹7,283 |
| [Crucial P2 500GB NVMe](https://computify.in/products/crucial-p2-500gb-pcie-3-0-3d-nand-nvme-m-2-with-enclosure-used-ssd) | 500GB | ₹5,699 | + ₹1,584 | ~₹7,283 |
| [BIWIN 512GB NVMe Gen3](https://computify.in/products/biwin-512gb-ap423-nvme-m-2-2280-gen-3-internal-ssd-used-ssd) | 512GB | ₹4,499 | + ₹1,584 | ~₹6,083 |

### Option B: NVMe SSD + Adapter

Use a standard M.2 NVMe SSD with a **Sintech** or **RIITOP** adapter.

#### Adapters

| Adapter | Price | Link |
|---------|-------|------|
| **Sintech** (B07FYY3H5F) | ₹1,584 | [Amazon.in](https://www.amazon.in/dp/B07FYY3H5F) |
| **RIITOP** (B09YCTVJ94) | ₹2,407 | [Amazon.in](https://www.amazon.in/dp/B09YCTVJ94) |

#### Compatible SSDs

| SSD | Capacity | Price | Store | Notes |
|-----|----------|-------|-------|-------|
| Samsung 980 | 500GB | ₹8,179 | [Flipkart](https://www.flipkart.com/samsung-980-500-gb-laptop-desktop-internal-solid-state-drive-ssd-mz-v8v500bw/p/itmca7041fe49d91) | Proven compatible with MBA 2015 (MacRumors confirmed) |
| Samsung 980 | 1TB | ₹16,199 | Flipkart | Same compatibility |
| Kingston NV3 | 1TB | ₹11,500 | [Flipkart](https://www.flipkart.com/kingston-nv3-1-tb-desktop-laptop-all-one-pc-s-blue-pcie-nvme-internal-solid-state-drive-ssd-snv3s-1000g/p/itm32cf4cdd194ee) | Budget pick, 5yr warranty |
| Kingston NV3 | 1TB | ₹17,511 | [PrimeABGB](https://www.primeabgb.com/online-price-reviews-india/kingston-nv3-1tb-pcie-gen-4-0-nvme-ssd-snv3sm3-1t0) | Alternative retailer |

#### Incompatible SSDs

- **WD Blue SN570 / SN770** — Not compatible with Sintech adapter

---

## Pricing Summary

| Option | Total (incl. adapter if needed) | Link |
|--------|-------------------------------|------|
| Apple Original 128GB (SparesOnly, direct swap) | **₹4,720** | [SparesOnly](https://www.sparesonly.in/products/macbook-air-13-a1466-early-2015-2016-2017-128gb-256gb-512gb-ssd) |
| Apple Original 512GB (SparesOnly, direct swap) | **₹8,850** | [SparesOnly](https://www.sparesonly.in/products/macbook-air-13-a1466-early-2015-2016-2017-128gb-256gb-512gb-ssd) |
| BIWIN 512GB NVMe (Computify) + Sintech | **~₹6,083** | [Computify](https://computify.in/products/biwin-512gb-ap423-nvme-m-2-2280-gen-3-internal-ssd-used-ssd) |
| Crucial P1/P2 500GB NVMe (Computify) + Sintech | **~₹7,283** | [Computify](https://computify.in/collections/buy-used-ssd) |
| Samsung 980 500GB (Flipkart, new) + Sintech | **~₹9,763** | [Flipkart](https://www.flipkart.com/samsung-980-500-gb-laptop-desktop-internal-solid-state-drive-ssd-mz-v8v500bw/p/itmca7041fe49d91) |
| Kingston NV3 1TB (Flipkart, new) + Sintech | **~₹13,084** | [Flipkart](https://www.flipkart.com/kingston-nv3-1-tb-desktop-laptop-all-one-pc-s-blue-pcie-nvme-internal-solid-state-drive-ssd-snv3s-1000g/p/itm32cf4cdd194ee) |
| Samsung 980 1TB (Flipkart, new) + Sintech | **~₹17,783** | [Flipkart](https://www.flipkart.com/samsung-980-500-gb-laptop-desktop-internal-solid-state-drive-ssd-mz-v8v500bw/p/itmca7041fe49d91) |

---

## Installation Steps

1. **Tools needed:** P5 Pentalobe screwdriver
2. Power down completely
3. Remove 10 bottom case screws (2× 9mm, 8× 2.6mm)
4. Pop off lower case
5. Disconnect battery connector
6. Unscrew and slide out existing SSD
7. **If using adapter:** Attach NVMe SSD to adapter, install adapter
8. **If using Apple SSD:** Direct drop-in
9. Secure with screw
10. Reconnect battery, replace bottom case
11. Boot to **Internet Recovery** (Cmd+Option+R)
12. Use Disk Utility to format new SSD (APFS/GUID partition map)
13. Reinstall macOS

---

## Post-Installation Notes

- **Hibernation:** Some MacBook Air models may experience kernel panics with hibernation. Disable hibernation if issues occur: `sudo pmset -a hibernatemode 0`
- **TRIM:** Enable TRIM for third-party NVMe SSDs: `sudo trimforce enable`
- **Boot Camp:** Windows installation via Boot Camp may have issues with NVMe drives. Not recommended for dual-boot.

---

## Other Upgrade Possibilities

Beyond the SSD, here's what can and cannot be upgraded on the MacBook Air 13" Early 2015:

### Upgradeable ✓

| Component | Details | Notes |
|-----------|---------|-------|
| **SSD** | Apple OEM blade or NVMe + adapter | Covered above |
| **Battery** | A1495 (7.5V 54.3Wh) | Replacement costs ~₹3,000-5,000 in India. If yours holds <80% capacity, replace it for better battery life |
| **Wi-Fi/Bluetooth Card** | BCM94360CS2 (part #661-7465) | Same card across 2013-2017 models. Replacement can fix connectivity issues, but **Wi-Fi 6 (AX) upgrade is not possible** — no macOS drivers exist for Intel AX200/AX210 |

| **Thermal Paste** | CPU/heat sink | Old paste dries out. Reapplying can reduce fan noise and improve sustained performance |
| **Logic Board Swap** | i5 1.6GHz → i7 2.2GHz (820-00165-A) | All 2013-2017 A1466 boards are interchangeable. Gives ~30% CPU gain. RAM stays 8GB. See full section below |
| **Fan** | 5V 0.5A fan | Replace if noisy or failing |
| **Speakers / Trackpad / Keyboard** | Bolt-on parts | All replaceable with standard tools |
| **macOS (OpenCore Legacy Patcher)** | Run unsupported macOS versions | MBA 2015 caps officially at Monterey (12). OCLP can install Ventura/Sonoma/Sequoia with working graphics acceleration |

### Not Upgradeable ✗

| Component | Reason |
|-----------|--------|
| **RAM** | Soldered (LPDDR3 8GB). BGA rework to 16GB is technically possible but requires microsoldering, resistor re-mapping, and costs more than the laptop is worth |
| **CPU** | Soldered (BGA). Replacing the CPU requires a BGA rework station and BIOS reprogramming — impractical for most users |
| **Display** | Not upgradable to higher resolution/refresh rate (but can be replaced if damaged) |
| **GPU** | Intel HD Graphics 6000 — integrated on CPU, not upgradeable |

### Recommended Order of Upgrades

1. **SSD upgrade** (biggest performance improvement)
2. **Battery replacement** (if degraded)
3. **Thermal paste reapplication** (if fans run loud)
4. **OpenCore Legacy Patcher** (to run newer macOS)
5. **Logic board swap to i7** (only if you find a good deal on a used board)

---

## Logic Board Swap: i5 → i7 Upgrade

### Compatibility

All A1466 (2013-2017) logic boards are fully interchangeable with each other. The 2012 A1466 is slightly different (shorter webcam cable), but 2013-2017 use the same connectors, mounting points, and I/O layout.

The board you want for the **Early 2015** model is the **820-00165-A** (PPN) / **661-02394** (APN). It has:
- **CPU:** 2.2GHz Intel Core i7-5650U (vs your current 1.6GHz i5-5250U — ~30% faster)
- **RAM:** 8GB LPDDR3 1600MHz (same as your current board)
- **GPU:** Intel HD Graphics 6000 (same)
- **Includes:** Heatsink (comes with the board)

### Performance gain

| CPU | Geekbench 5 Single | Geekbench 5 Multi | Cinebench R23 Multi |
|-----|-------------------|-------------------|-------------------|
| i5-5250U (1.6GHz) | ~680 | ~1,450 | ~1,650 |
| i7-5650U (2.2GHz) | ~790 | ~2,020 | ~2,420 |
| **Gain** | **+16%** | **+39%** | **+47%** |

The i7 has a higher base clock (2.2GHz vs 1.6GHz) and higher turbo (3.2GHz vs 2.7GHz), so multi-threaded tasks benefit significantly. Single-threaded feels snappier but not transformative.

### Is it worth it?

- **If your current board works:** Probably not. The i7 is 30-40% faster on paper, but in daily use (browsing, docs, light coding) the difference is modest. Better to spend on SSD + battery.
- **If your current board is dead/failing:** Yes, it makes sense to replace with i7 rather than i5 if you can find one at a reasonable price.

### Sourcing options (ranked by total cost to India)

| # | Source | Board Price | Shipping | Customs | Est. Total in ₹ | Link |
|---|--------|------------|----------|---------|----------------|------|
| 1 | **UsedMac.com** (US) | $85 (~₹7,100) | ~$20-30 | ~40% | **~₹10-12k** | [661-02394](https://usedmac.com/product/661-02394/) |
| 2 | **OLX / FB Marketplace** (India) | ₹6-15k | Free | None | **₹6-15k** | Search "A1466 for parts" |
| 3 | **Tekdep** (US) — 1.7GHz i7 | $59.77 (~₹5k) | ~$15-25 | ~40% | **~₹8-10k** | [820-3437-B i7](https://tekdep.com/product/a1466-original-logic-board-1-7ghz-i7-8gb-820-3437-b-for-2013-2014-macbook-air-13) |
| 4 | **TechToro/MacNest** (US) | $149.99 (~₹12.5k) | ~$15-25 | ~40% | **~₹16-18k** | [661-02394](https://techtoro.io/macbook-air/macbook-air-13-a1466/macbook-air-13-2017/logic-board-i7-2-2ghz-8gb-661-02394-a1466-2015-2017) |
| 5 | **AliExpress** (China) | ~$142 (~₹12k) | Free/cheap | ~40% | **~₹16-18k** | [Search](https://www.aliexpress.com/w/wholesale-820-00165-a-logic-board.html) |
| 6 | **eBay** (Global) | $85-150 | ~$20-30 | ~40% | **~₹12-18k** | [Search](https://www.ebay.com/shop/macbook-air-logic-board-a1466) |
| 7 | **Beetstech** (US) | $229 (~₹19k) | Free | ~40% | **~₹22-24k** | [661-02394](https://beetstech.com/product/macbook-air-13-inch-a1466-logic-board-661-02394) |
| 8 | **SparesOnly i5** (India) | ₹13,750-14,750 | Free | None | **₹13,750-14,750** | [i5 board](https://www.sparesonly.in/products/macbook-air-13-a1466-2012-2017-1-8-ghz-logic-board) |

### Detailed source notes

**UsedMac.com (Best value)** — Has 1,433 units in stock of the exact 661-02394 (2.2GHz i7, 8GB) at $85. Ships via UPS or US Mail. To get an India shipping quote: email `info@usedmac.com` with your address. 90-day warranty. At this price even after shipping + customs (~40%), it's ~₹10-12k — cheaper than SparesOnly's i5.

**OLX / FB Marketplace (Donor laptop route)** — Search for "A1466 for parts" or "MacBook Air dead motherboard". An i5 donor typically goes for ₹5-7k. An i7 donor is rarer (i7 was a BTO option). Ask sellers for the serial number — you can decode it to check if it's i7. If you find one under ₹10k, this is the cheapest option.

**AliExpress** — Many sellers list "820-00165-A i7 2.2GHz 8GB" for ~$142. AliExpress Standard Shipping to India: 15-40 days free. Orders under ₹5,000 often clear customs without duty, but an ₹12,000 board will almost certainly be assessed: BCD ~15% + IGST 18% = ~35-40% additional. Track via India Post after it hits customs.

**Beetstech (Best warranty)** — $229 but includes free shipping and a **lifetime warranty**. If you plan to keep the laptop long-term, the peace of mind may be worth the premium. Ships worldwide.

### Installation notes

1. Remove bottom case (P5 Pentalobe)
2. Disconnect battery
3. Disconnect: I/O flex cable, display cable, webcam cable, Wi-Fi antenna cables, speaker cable, fan cable
4. Remove logic board screws (3x Phillips)
5. Lift board out gently
6. Transfer your existing SSD and thermal pad to new board (the i7 board includes a heatsink)
7. Reverse steps to reassemble
8. The board will boot with your existing SSD and macOS — no reinstall needed

## Market Context (July 2026)

A global NAND flash shortage has inflated SSD prices 2-3x above historical norms. Budget NVMe SSDs like the Crucial P3, Samsung 970 EVO Plus, and Lexar NM610 are either out of stock or priced significantly higher than their usual rates on both Amazon.in and Flipkart.

---

---

## Linux / Fedora Compatibility

The MacBook Air 13" Early 2015 (A1466) works well under Linux. Here's what you can expect with **Fedora 41** (or recent Fedora releases):

### What works out of the box ✓

| Component | Status | Notes |
|-----------|--------|-------|
| **Wi-Fi** | ✓ | BCM4360 (broadcom-wl driver in Fedora non-free repos) |
| **Bluetooth** | ✓ | BCM20702 — works after firmware loaded |
| **Trackpad** | ✓ | Multi-touch gestures, click, tap-to-click work with `libinput` |
| **Keyboard** | ✓ | Full function keys, brightness controls |
| **Display** | ✓ | Native 1440×900, backlight control works |
| **Audio** | ✓ | Built-in speakers, headphone jack |
| **Camera** | ✓ | 720p FaceTime webcam (USB device) |
| **USB Ports** | ✓ | Both USB 3.0, USB-C via Thunderbolt 2 adapter |
| **Thunderbolt 2** | ✓ | Mini DisplayPort output, daisy chaining |
| **Suspend/Resume** | ✓ | S3 sleep works |
| **Battery Reporting** | ✓ | Charge level, cycles, health via `upower` |

### What needs manual setup ⚠

| Component | Notes |
|-----------|-------|
| **Wi-Fi** | On Fedora, install `broadcom-wl` driver from RPM Fusion non-free repo. The open-source `b43` driver has poor performance. |
| **Fan control** | MacBooks use SMC for fan control. `mbpfan` daemon works well — install via `sudo dnf install mbpfan` |
| **Keyboard backlight** | Works but brightness adjustment may need `echo N > /sys/class/leds/smc::kbd_backlight/brightness` |

### Known issues

- **Suspend to idle** (s2idle) is default on some kernels and drains battery. Ensure S3 (deep) sleep: `cat /sys/power/mem_sleep` — set with `sudo grubby --args="mem_sleep_default=deep" --update-kernel=DEFAULT`
- **Thunderbolt security level** may need setting in BIOS for some docks
- **CPU throttling** under sustained load — old thermal paste can cause this. Consider repasting
- **Feedbackd** (haptic feedback) does not work — the MacBook Air doesn't have a haptic engine, only a physical click

### Fedora 41 specific notes

- **ISO size**: ~2.5GB. Write with `dd` or Fedora Media Writer
- **Live USB performance**: Runs entirely from RAM. Will feel slower than installed OS due to USB 2.0/3.0 read speeds and lack of swap. Install to SSD for real performance
- **Battery life**: ~4-5 hours on Fedora with `powertop --auto-tune` vs ~7-8 hours on macOS. The `broadcom-wl` driver uses more power than macOS's native driver
- **OpenCore Legacy Patcher note**: If you dual-boot, OCLP + Linux can coexist but may need SecureBoot disabled

### Performance comparison (on same hardware)

| Workload | Fedora 41 (live USB) | Fedora 41 (installed SSD) | macOS Monterey |
|----------|---------------------|--------------------------|----------------|
| Boot time | ~45-60s (USB 3.0) | ~15s | ~20s |
| App launch (Firefox) | ~5-8s | ~2s | ~2s |
| Memory use (idle) | ~1.2GB | ~1GB | ~2.5GB |
| Battery (light use) | ~3-4h | ~4-5h | ~7-8h |

> **Bottom line:** Linux runs great on this hardware once installed. The live USB experience is not representative of installed performance. If you're choosing between macOS and Linux, Fedora gives you a modern, well-supported desktop on a machine Apple has dropped from official support.

---

## Resources

- [iFixit Guide: MacBook Air 13" Early 2015 SSD Upgrade to NVMe](https://www.ifixit.com/Guide/MacBook+Air+13-Inch+Early+2015+SSD+Upgrade+to+NVMe/119755)
- [MacRumors Forums: Upgrading 2013-2015 MacBook Pro SSD to M.2 NVMe](https://forums.macrumors.com/threads/upgrading-2013-2015-macbook-pro-ssd-to-m-2-nvme.2034976/)
- [Ubuntu Wiki: MacBookAir7,2](https://wiki.ubuntu.com/HardwareSupport/MacBookAir7-2)
- [Arch Wiki: MacBook Air 7,2](https://wiki.archlinux.org/title/MacBook_Air_7,2)

---

*Generated on 23 July 2026*
