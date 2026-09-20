# 🧪 QA Portfolio - Manual Testing

 repository นี้จัดทำขึ้นเพื่อนำเสนอผลงานและทักษะด้าน **Manual Testing** ผ่านโปรเจกต์ทดสอบเว็บแอปพลิเคชันจำลองเพื่อเตรียมความพร้อมสำหรับการทำงานจริงและการสมัครงานสหกิจศึกษา

---

## 🎯 Project: The Internet
โปรเจกต์นี้เป็นการทดสอบระบบเว็บแอปพลิเคชันเพื่อสาธิตและฝึกฝนทักษะการทำ **Manual Testing** พื้นฐาน ตั้งแต่การออกแบบเคส การทดสอบฟังก์ชัน การจับบั๊ก และการทำเอกสารรายงานผล

### 🛠️ Testing Skills (ทักษะการทดสอบ)
- 📝 **Test Case Design** (การออกแบบเคสการทดสอบ)
- ⚙️ **Functional Testing** (การทดสอบฟังก์ชันการทำงานของระบบ)
- 🐛 **Bug Reporting** (การรายงานและบันทึกบั๊ก)
- 📄 **Test Documentation** (การจัดทำเอกสารการทดสอบอย่างเป็นระบบ)

### 🧰 Tools Used (เครื่องมือที่ใช้)
- **Microsoft Excel** (จัดทำเอกสาร Test Case และ Bug Report)
- **GitHub** (ระบบจัดเก็บและนำเสนอ Portfolio)

---

## 📦 Deliverables (สิ่งที่จัดทำในโปรเจกต์)
- 📝 **Test Case:** เคสการทดสอบที่ครอบคลุมเงื่อนไขต่างๆ ของระบบ
- 🐛 **Bug Report:** รายงานปัญหาที่พบพร้อมรายละเอียดและระดับความสำคัญ
- 📸 **Screenshot Evidence:** ภาพถ่ายหน้าจอหลักฐานการทดสอบและการเกิดบั๊ก

---

## 📁 Files in Repository (รายการไฟล์ใน คลังข้อมูล)

คุณสามารถดูรายละเอียดของเอกสารการทดสอบทั้งหมดได้จากไฟล์ภายใน Repository นี้:

- 📊 **`TestCase_TheInternet.xlsx`** – เอกสารรายละเอียด Test Case
Test Case ID	ชื่อทดสอบ	ขั้นตอนการทำ	ผลที่คาดหวัง	ผลที่ได้จริง	ผ่าน/ไม่ผ่าน	หมายเหตุ																			
Test Case ID TC_001	Login ด้วย Username ผิด เเละ Password	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. กรอก Username: ผิดๆ (หรืออะไรก็ได้ที่ผิด)
3. กรอก Password: อะไรก็ได้
4. กดปุ่ม Login"	เข้าสู่ระบบไม่สำเร็จ เเละเห็นข้อความ "Your username is invalid!" ควรขึ้นข้อความกรอกข้อมูลผิด	เข้าสู่ระบบไม่สำเร็จ เเละเห็นข้อความ "You logged into a secure area!" (ตรงตามที่คาดหวัง)	ไม่ผ่าน																				
Test Case ID TC_002	Login ด้วย Username เเละ Password ที่ถูกต้อง	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. กรอก Username: tomsmith
3. กรอก Password: SuperSecretPassword!
4. กดปุ่ม Login"	เข้าสู่ระบบสำเร็จ เเละเห็นข้อความ "You logged into a secure area!"	เข้าสู่ระบบสำเร็จ เเละเห็นข้อความ "You logged into a secure area!"(ตรงตามที่คาดหวัง)	ผ่าน																				
Test Case ID TC_003	Login โดยไม่กรอกอะไรเลย	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. ไม่กรอกอะไรเลย"	ควรขึ้นข้อความเเจ้งเตือน ให้กรอก Username เเละ Password	เข้าสู่ระบบไม่สำเร็จ ไม่ขึ้น "You logged into a secure area!" (ตามที่คาดหวัง)	ไม่ผ่าน																				
Test Case ID TC_004	ใส่เเค่ Username	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. ใส่เเค่ Username (ชื่ออะไรก็ได้)"	ควรขึ้นข้อความเเจ้งเตือน ให้กรอก Password	ข้าสู่ระบบไม่สำเร็จ ไม่ขึ้น "You logged into a secure area!" เเละชื่อที่พิมพ์ไปหาย (ตามที่คาดหวัง)	ไม่ผ่าน																				
Test Case ID TC_005	กดปุ้ม Logout หลัง Login เสร็จ	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. กรอก Username: tomsmith
3. กรอก Password: SuperSecretPassword!
4. กดปุ่ม Login 5.เเละกด Logot"	เข้าสู่ระบบสำเร็จ เเละเห็นข้อความ "You logged into a secure area!" เข้าหน้าLogout เเล้วกด ก็เข้า Login เหมือนเดิมเเละให้กรอกใหม่	เข้าสู่ระบบสำเร็จ เเละเห็นข้อความ "You logged into a secure area!" เข้าหน้าLogout เเล้วกด ก็เข้า Login เหมือนเดิม (ตามที่คาดหวัง)	ผ่าน																				
- 🐛 **`BugReport_TheInternet.xlsx`** – เอกสารรายงานบั๊กที่พบในระบบ

  BUG ID	หัวข้อ	Severity	Priority	ขั้นตอนทำซ้ำ	ผลที่คาดหวัง	ผลที่ได้จริง
BUG_001	ปุ่ม Login กดเเล้วไม่ทำงานเมื่อกรอกข้อมูลว่าง	Medium ปานกลาง	High	1. เปิดเว็บ https://the-internet.herokuapp.com/login 2.ไม่กรอกอะไรเลย 3.กดปุ่ม Login	ควรขึ้นข้อความเเจ้งเตือนว่าต้องกรอกข้อมูล	ไม่มีข้อความอะไรขึ้นเลย
ฺBUG_002	กรอก Username ถูก เเต่ Password รหัสไม่ถูก	Medium ปานกลาง	Medium	1. เปิดเว็บ https://the-internet.herokuapp.com/login 2.กรอก Username ถูก  เเต่ Password รหัสไม่ถูก 3.กดปุ่ม Login	ควรขึ้นข้อความ ว่ารหัสไม่ถูกต้อง  เฉพาะ Password ต้องกรอกใหม่อีกครั้ง	ไม่มีข้อความอะไรขึ้นเลย
BUG_003	ไม่มีข้อความแจ้งเตือนเมื่อกรอกเฉพาะ Username โดยไม่กรอก Password	Medium ปานกลาง	Medium	"1. เปิดเว็บ https://the-internet.herokuapp.com/login
2. กรอก Username: tomsmith
3. ไม่กรอก Password
4. กดปุ่ม Login"	ควรขึ้นข้อความแจ้งเตือนว่าต้องกรอก Password	ม่มีข้อความแจ้งเตือนอะไรขึ้นเลย


