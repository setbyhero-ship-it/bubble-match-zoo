# 🫧 Bubble Match! Zoo Edition

เกมจับคู่ฟองสบู่น่ารัก สไตล์ Zoo · สร้างรายได้จากโฆษณา Rewarded Video

## วิธีเล่น

1. เปิด `bubble-match-zoo.html` ในเบราว์เซอร์
2. เลือกระดับความยาก
3. พลิกฟองเพื่อจับคู่ตัวละครให้ครบก่อนเวลาหมด
4. ใช้ Power-up เมื่อจำเป็น (ดูโฆษณาสั้น ๆ เพื่อรับ)

## ไฟล์ในโปรเจกต์

```
📁 Matching game/
├── bubble-match-zoo.html   ← เกมหลัก (HTML5 Prototype)
├── game_design_overview_final.html  ← Design Overview
└── README.md               ← ไฟล์นี้
```

## Design Decisions

| หัวข้อ | ตัวเลือก |
|--------|---------|
| Art Style | Bubble Character (3D glossy spheres) |
| Background | Zoo (สวนสัตว์ animate) |
| Menu | Dark Glass Morphism |
| ภาษา | ไทย |
| Platform (ต่อไป) | Flutter + AdMob |

## ระดับความยาก

| ด่าน | Grid | เวลา |
|------|------|------|
| ง่าย | 3×4 | 90 วิ |
| ปกติ | 4×4 | 75 วิ |
| ยาก | 4×5 | 60 วิ |
| นรก | 4×6 | 45 วิ |

## Power-ups

| Power-up | เอฟเฟค | ชาร์จ |
|----------|--------|-------|
| ⏱️ เพิ่มเวลา | +15 วินาที | 2 |
| 👁️ แอบดู | เปิดดูหมด 1.8 วิ | 2 |
| 💥 จับคู่ให้ | Auto 1 คู่ | 1 |
| ❄️ หยุดเวลา | หยุดนับ 5 วิ | 1 |

## ขั้นต่อไป → Flutter App

```bash
# ติดตั้ง Flutter
https://flutter.dev/docs/get-started/install

# สร้าง Project
flutter create bubble_match_zoo

# dependencies ที่ต้องใช้
google_mobile_ads: ^5.x   # AdMob
flame: ^1.x               # Game engine (optional)
```

## Revenue Model

- 🎬 **Rewarded Video** (หลัก) — ดูโฆษณาแลก Power-up · RPM $2–5
- 📋 **Interstitial** — ระหว่างด่าน ทุก 3–5 Level · RPM $1–3
- 🏷️ **Banner** — หน้า Menu เท่านั้น · RPM $0.3–0.8
