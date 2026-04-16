# Gangneung Accommodation Report — Apr 19–26, 2026

**Trip parameters**
- 7 nights · Sun Apr 19 → Sun Apr 26, 2026
- 4 adults (possibly 5–6 if extended family joins)
- Preferred areas: Gyeongpo-dong (경포동), Chodang-dong (초당동), near 강릉역
- Budget: ₩80K–130K/night, target ≤₩700K total
- Must-haves: entire place, 2+ bedrooms, kitchen, washer, parking
- FX rate: 1 USD = ₩1,475.27 (live, 2026-04-16)

---

## ⚠ Critical data-quality findings from detail-page deep-dive

The original card-level scrape produced false positives. After visiting detail pages for the top 5 candidates:

| Originally claimed | Actual reality |
|---|---|
| "Airbnb ₩692K 2br entire place in Gangneung" | Property is actually in **양양 (Yangyang)**, a neighboring region — Airbnb search leaked outside Gangneung |
| "강릉 경포 오션힐펜션 ₩686K Tier 1 pick" | **Single pension-style hotel room**, not 2br entire unit. No washer. Address is **안현동**, not 경포동 |
| "강릉 더원펜션 ₩728K" | Same pattern — pension room, not entire unit. No washer confirmed |

**Implication:** "펜션" on Korean OTAs (Goodchoice, Trip.com, etc.) frequently means a **pension-style hotel room**, not a rental house with bedrooms. The card-level data can't distinguish — only the detail page can.

---

## ✅ Tier 1 — Verified all must-haves (entire place + 2+ br + kitchen + washer + parking)

| # | Property | Total KRW | ~USD | /nt | Br | ⭐ (reviews) | Area | Verified | Source |
|---|---|---|---|---|---|---|---|---|---|
| 1 | **Airbnb 황토찜질방 5br** | ₩744,731 | $505 | ₩106,390 | **5br** | 5.0 (11) | Jumunjin outskirts (5 min drive to Yeongjin Beach) | ✓ entire house, K/W/P + ondol 찜질방 + BBQ + AC | [Airbnb /rooms/1445345613923327667](https://www.airbnb.com/rooms/1445345613923327667) |
| 2 | **Airbnb 사천해변 풀옵션 투룸 아파트** | ₩903,812 | $613 | ₩129,116 | 2br | 5.0 (12) | 사천해변 (1-min walk to beach) | ✓ entire apt, K/W + **dryer** + P + ondol + AC | [Airbnb /rooms/1544199861394746225](https://www.airbnb.com/rooms/1544199861394746225) |

**#1 hits ₩744K — 6% over your ₩700K stretch target, but best option for 5–6 guests and remains under ₩130K/nt.**

---

## 🔍 Tier 2 — Unverified but promising (card-level data only)

These passed initial filters but need detail-page verification before booking. Pattern concern: may be single pension rooms, not entire units.

### New Gyeongpo candidates (Goodchoice v2 re-scrape, pension filter properly applied)

| # | Property | /nt | Total | ⭐ (reviews) | Distance to 경포해변 | Note |
|---|---|---|---|---|---|---|
| 3 | **강릉 KN하우스** | ₩86,731 | **₩607K** | 9.8 (402) | 3-min drive | Cheapest Gyeongpo option — ~$411 |
| 4 | **강릉 까사드마르** | ₩118,857 | ₩832K | **9.9 (383)** | 2-min drive | Highest-rated Gyeongpo pension |

### New Gyeongpo candidates (Trip.com — our Agoda alternative)

| # | Property | /nt | Total | ⭐ | Link |
|---|---|---|---|---|---|
| 5 | **Gyeongpoen Pension** | ₩86,818 | ₩608K | 9.2 | [Trip.com/38009777](https://www.trip.com/hotels/detail/?hotelId=38009777) |
| 6 | **Gangneung Gyeongpodae Jajaknamu** | ₩93,012 | ₩651K | 9.4 | [Trip.com/33545665](https://www.trip.com/hotels/detail/?hotelId=33545665) |
| 7 | **Gangneung Dabian Spa Pension** | ₩106,376 | ₩745K | 10.0 | [Trip.com/33477253](https://www.trip.com/hotels/detail/?hotelId=33477253) |

### 초당동 options (Naver discovery, priced via Yanolja cross-reference)

0/10 matched on Goodchoice; 7/10 priced on Yanolja.

| Property | /nt | Total | Note |
|---|---|---|---|
| **더강문풀빌라** | ₩112,100 | ₩785K | Pool villa — strong group amenity fit |
| **강릉비치힐펜션** | ₩119,000 | ₩833K | "비치힐" branding suggests sea-view positioning |
| **상상초당** | ₩169,200 | ₩1,185K | Premium, over budget |
| 경포의휴일 / 스테이어스펜션 | ₩42–44K | ₩294–308K | ⚠ Suspiciously cheap — likely base rate that scales with guest count. Verify before trusting |

**3 Naver-only pensions** (not on any OTA, direct-booking required): 더초당펜션, 라온 바닷가 펜션, 담높은집

---

## 🥉 Tier 3 — Cheapest overall (but farther from target area)

| Property | Total | ~USD | Area | Note | Source |
|---|---|---|---|---|---|
| **강릉 더영진풀빌라펜션** | ₩623,000 | $422 | 연곡 (Yeongok) | 20+ km from Gyeongpo — pool villa, ocean view, ⭐5.0 | Yanolja |
| **강릉 썬리치펜션** | ₩654,500 | $443 | ocean view | ⭐5.0 | Yanolja |
| **강릉 더강릉오션스테이 First** | ₩665,000 | $451 | 사천진해변 | ⭐5.0 on Yanolja — **₩133K/nt on Goodchoice, so book via Yanolja** | Yanolja |

---

## Cross-site price discrepancy (verified)

Same property can differ substantially across OTAs. Always check multiple:

| Property | Yanolja | Goodchoice | Gap |
|---|---|---|---|
| 강릉 더강릉오션스테이 First | ₩95K/nt | ₩133K/nt | **₩38K/nt** (~40% diff) |

---

## Scrape coverage

| Site | Listings | Status | Notes |
|---|---|---|---|
| Airbnb | 24 | ✅ full | Yangyang listings leak through "Gangneung" search — verify address |
| Booking.com | 25 | ✅ full | |
| Yanolja | 40 | ✅ full | Best source for 초당동 pensions |
| Naver Map | 152 | ⚠ names only | Best neighborhood tags of any site (동 admin level) |
| Goodchoice (v1) | 10 | ❌ filter broken | Only 3 pensions; `accommodationType=pension` URL param cosmetic |
| **Goodchoice (v2)** | **40** | ✅ full | Fix: click 펜션 radio in sidebar UI, not URL param |
| Trip.com | 25 | ✅ full | Correct city ID is **61325** (not 1501043); use `/htls/getKeyWordSearch` autocomplete |
| Agoda | 0 | ❌ blocked | PAPI 400 — session-token / anti-bot |

## Detail-page deep-dive (5 candidates)

All 5 top-ranked Tier 1 candidates verified. 2 passed all must-haves, 3 failed.

---

## Must-verify gaps remaining

- **Entire-unit status unverified** for all Goodchoice v2 / Trip.com Tier 2 picks (KN하우스, 까사드마르, Gyeongpoen, Jajaknamu, Dabian)
- **Bedroom counts** unverified on everything except the 2 Airbnb verified picks
- **Wifi speed** — "기가" mentioned on 2 detail pages (including 오션힐 and the 양양 listing); others unknown
- **연박할인 (7-night discount)** not found on any of the 5 detail-page verified listings
- **Naver-only pensions** (더초당펜션, 라온 바닷가 펜션, 담높은집) need direct-call verification

---

## Bottom-line recommendations

**If you want absolute certainty about must-haves:** book **Airbnb 황토찜질방 5br** at ₩744,731 total (~$505). It's slightly over the ₩700K stretch target but verified to have everything. Particularly strong if extended family joins — 5 bedrooms + wide parking + ondol sauna.

**If 경포동 is non-negotiable and you'll accept a pension-room:** **강릉 KN하우스 (₩607K)** or **Gyeongpoen Pension (₩608K)** both offer Gyeongpo-adjacent stays under budget at ⭐9.2–9.8 ratings — but you must do a detail-page check first to confirm whether they're actually 2-bedroom entire units or single pension rooms.

**If you want beachfront:** **Airbnb 사천해변 투룸** at ₩904K — 1 min walk to Sacheon Beach, fully verified, 2br entire apt with washer/dryer, but 29% over budget target.

**Before booking:** cross-check the exact same property name across Yanolja + Goodchoice + Trip.com — the 40% price gap seen on 더강릉오션스테이 First is real.

---

*Data at `/home/jin/gangneung-scrape/*.json` + screenshots `*_screenshot.png`. Skill backing this research: https://github.com/jinpyo-jeon/claude-travel-research-skill*
