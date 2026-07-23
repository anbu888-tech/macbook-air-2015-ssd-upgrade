# MacBook Air 13" Early 2015 (A1466) SSD Upgrade Guide

Comprehensive documentation for upgrading the SSD in a **MacBook Air 13" Early 2015 (Model A1466 / MacBookAir7,2)**.

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

## Market Context (July 2026)

A global NAND flash shortage has inflated SSD prices 2-3x above historical norms. Budget NVMe SSDs like the Crucial P3, Samsung 970 EVO Plus, and Lexar NM610 are either out of stock or priced significantly higher than their usual rates on both Amazon.in and Flipkart.

---

## Resources

- [iFixit Guide: MacBook Air 13" Early 2015 SSD Upgrade to NVMe](https://www.ifixit.com/Guide/MacBook+Air+13-Inch+Early+2015+SSD+Upgrade+to+NVMe/119755)
- [MacRumors Forums: Upgrading 2013-2015 MacBook Pro SSD to M.2 NVMe](https://forums.macrumors.com/threads/upgrading-2013-2015-macbook-pro-ssd-to-m-2-nvme.2034976/)

---

*Generated on 23 July 2026*
