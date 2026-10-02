# 🎬 Movie & Series Watchlist

เว็บแอปสำหรับบันทึกและติดตามหนัง/ซีรีส์ที่อยากดูหรือดูแล้ว

## คุณสมบัติ
- เพิ่ม/ลบ/แก้ไขรายการหนังและซีรีส์
- ติดตามสถานะการดู (ดูแล้ว/กำลังดู/ยังไม่ดู)
- จัดเก็บข้อมูลผ่าน REST API

## เทคโนโลยีที่ใช้
- Node.js + Express
- HTML, CSS, JavaScript (Vanilla)
- Nodemon (สำหรับ development)

## การติดตั้ง

\`\`\`bash
# Clone โปรเจกต์
git clone <repository-url>

# เข้าไปที่โฟลเดอร์โปรเจกต์
cd MovieWatchlist

# ติดตั้ง dependencies
npm install
\`\`\`

## การใช้งาน

\`\`\`bash
# รัน development server
npm run dev
\`\`\`

จากนั้นเปิดเบราว์เซอร์ไปที่:
\`\`\`
http://localhost:3000
\`\`\`

## โครงสร้างโปรเจกต์

\`\`\`
MovieWatchlist/
├── server/
│   └── server.js       # Express server
├── public/
│   ├── index.html      # หน้าเว็บหลัก
│   ├── style.css        # Styling
│   └── script.js        # Frontend logic
├── package.json
└── README.md
\`\`\`

## 🔗 API Endpoints

| Method | Endpoint           | คำอธิบาย                  |
|--------|---------------------|----------------------------|
| GET    | /api/movies         | ดึงรายการหนัง/ซีรีส์ทั้งหมด |
| GET    | /api/movies/:id     | ดึงข้อมูลหนังตาม ID       |
| POST   | /api/movies         | เพิ่มหนัง/ซีรีส์ใหม่       |
| PUT    | /api/movies/:id     | แก้ไขข้อมูลหนัง            |
| DELETE | /api/movies/:id     | ลบหนัง/ซีรีส์               |

## 🐛 ภาพหลักฐานการ Debug

### ภาพที่ 1: ทดสอบ GET /api/movies
![Debug Test 1](./screenshotsdebug1.png)

### ภาพที่ 2: ทดสอบ POST /api/movies
![Debug Test 2](./screenshotsdebug2.png)