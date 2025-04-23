# Thailand Location 77 Database [SQL Server]

📦 **ฐานข้อมูลประเทศไทย** สำหรับ SQL Server  
ครบถ้วนด้วย **รายชื่อจังหวัด อำเภอ ตำบล และรหัสไปรษณีย์** พร้อมภาษาอังกฤษ!  
เหมาะสำหรับงานระบบหลังบ้าน, แบบฟอร์มลงทะเบียน, GIS, และงานพัฒนาแอปพลิเคชัน

---

## ✅ รายละเอียดข้อมูล

- 🌍 **แบ่งภาค**: 6 ภาค
- 🏙️ **จังหวัด**: 77 จังหวัด (มีชื่อภาษาอังกฤษครบทุกจังหวัด)
- 🏞️ **อำเภอ**: 998 อำเภอ (มีชื่อภาษาอังกฤษ 729 อำเภอ)
- 🏡 **ตำบล**: 8,860 ตำบล
- ✉️ **รหัสไปรษณีย์** ครอบคลุมครบถ้วน

---

### ⚙ วิธีติดตั้ง (SQL Server)

#### 1. ตั้งค่า Collation

```sql
ALTER DATABASE YourDatabaseName COLLATE Thai_CI_AS;
```

> เปลี่ยน `YourDatabaseName` เป็นชื่อฐานข้อมูลของคุณ

---

#### 2. ใช้คำสั่ง `sqlcmd` เพื่อนำเข้าข้อมูล

```bash
sqlcmd -S "YourServer" -d "YourDatabase" -U "sa" -P "YourPassword" -i "thailand_sqlserver.sql" -f 65001
```

> 🔐 เปลี่ยน `"YourServer"`, `"YourDatabase"`, `"YourPassword"` และ path ของไฟล์ `.sql` ตามเครื่องคุณ

---

### 🙏 ขอบคุณแหล่งข้อมูลต้นฉบับ

- ข้อมูลต้นฉบับ (ภาษาไทย):  
  [AT12 @ ThaiCreate](https://www.thaicreate.com/member-profile/uid-100725.html)  
- ภาษาอังกฤษโดย:  
  [kongvut/thai-province-data](https://github.com/kongvut/thai-province-data)

---
