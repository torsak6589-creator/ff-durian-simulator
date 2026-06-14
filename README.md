# FF Durian — Break-Even Simulator 2569

> ระบบจำลองต้นทุน-กำไรทุเรียน สำหรับ บริษัท ห้องเย็นโชติวัฒน์หาดใหญ่ จำกัด (มหาชน)  
> Farm Code C-MTA จันทบุรี | ฤดูกาล 2569

## 🌐 เปิดใช้งาน

**👉 [เปิด Simulator](https://torsak6589-creator.github.io/ff-durian-simulator/)**

## ✨ ฟีเจอร์

| ตัวแปร | ปรับได้ | ช่วง |
|---|---|---|
| 📦 ปริมาณซื้อ | Slider + ปุ่ม ±100/±500 | 1,000–7,000 ตัน |
| 💰 ราคาซื้อ RM | Slider + ปุ่ม ±1/±5 | 35–75 ฿/kg |
| 🟢 Grade A % | Slider + ปุ่ม ±1/±5 | 20–80% |
| 🔵 Grade B % | Slider + ปุ่ม ±1/±5 | 5–40% |
| 💲 ราคาขาย | พิมพ์แก้ไขได้ทุกเกรด | A/B/C/BK/bk |
| 🔧 ต้นทุนผลิต | พิมพ์แก้ไขได้ | ฿/kg FG |

### ผลลัพธ์แบบ Real-Time
- Break-Even ราคาซื้อสูงสุด
- สถานะ ✅ กำไรดี / ⚠️ margin บาง / ❌ ขาดทุน
- สรุปผลประกอบการเต็มรูปแบบ (ลงทุน / รายได้ / กำไร)
- P&L ต่อ 100 kg สด + ต่อ kg FG
- Scenario Analysis ส่วนเหลือ
- Preset 7 สถานการณ์

## 🚀 วิธี Deploy

ไฟล์เดียว `index.html` — ไม่ต้องลง server, ไม่ต้อง build

### GitHub Pages (แนะนำ)
1. Fork หรือ Clone repo นี้
2. ไป Settings → Pages → Source: `main` / `root`
3. เปิดลิงก์ที่ได้

### อื่นๆ
- **SharePoint**: อัปโหลด index.html → แชร์ลิงก์
- **Google Drive**: อัปโหลด → เปิดด้วย Chrome
- **Internal Server**: วางไฟล์ใน web root

## 📐 สูตรคำนวณ

```
Flow: 100kg สด → 95kg (−5% ขนส่ง) → 85.5kg (−10% บ่ม) → 29.925kg FG (35% ปอก)
Overall Yield = 29.925%

BV (Blended Value) = Σ(Grade% × ราคาขาย) ถ่วงน้ำหนัก
Break-Even RM = (FG × BV − FG × ต้นทุนผลิต) ÷ 100
```

## 📄 License

Internal Use Only — บริษัท ห้องเย็นโชติวัฒน์หาดใหญ่ จำกัด (มหาชน)
