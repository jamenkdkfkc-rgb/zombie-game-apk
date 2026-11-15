วิธีสร้าง APK โดยใช้มือถือ Android และ GitHub Actions

1) แตกไฟล์ ZIP นี้ในมือถือ (แอป Files/ตัวจัดการไฟล์ > Extract)
2) เข้า https://github.com และสมัคร/เข้าสู่ระบบ
3) กด + > New repository ตั้งชื่อ เช่น zombie-game-apk แล้วเลือก Public (สะดวกสำหรับ workflow) > Create repository
4) ในหน้า repo กด Add file > Upload files แล้วอัปโหลดไฟล์/โฟลเดอร์ทั้งหมดจากโปรเจกต์ที่แตกแล้ว รวมโฟลเดอร์ .github ด้วย
   หมายเหตุ: ถ้าไม่เห็น .github ให้เปิดการแสดงไฟล์ซ่อนในแอปจัดการไฟล์
5) กด Commit changes
6) เปิดแท็บ Actions ใน repository ถ้าขึ้นคำถามให้ยืนยันเปิด workflows ให้กดยืนยัน
7) เลือก workflow ชื่อ Build Zombie Game APK > Run workflow > Run workflow
8) รอให้เสร็จ (เครื่องหมายเขียว) เปิดรายการงานที่สำเร็จ เลื่อนลงส่วน Artifacts แล้วกด zombie-game-apk เพื่อดาวน์โหลด ZIP
9) แตก ZIP artifact จะได้ app-debug.apk เปิดไฟล์ APK และกดติดตั้ง (อาจต้องอนุญาตติดตั้งแอปจากแหล่งนี้)

ข้อควรทราบ: APK นี้เป็น debug build สำหรับทดสอบเกม ไม่ใช่ APK ที่เซ็นสำหรับเผยแพร่ใน Play Store
