โปรเจกต์เตรียมแปลงเกม HTML เป็น Android APK

เกมต้นฉบับถูกเก็บไว้ที่ www/index.html

วิธีสร้าง APK (ต้องใช้คอมพิวเตอร์ Windows/Mac/Linux และติดตั้ง Node.js กับ Android Studio):
1) แตกไฟล์ ZIP
2) เปิด Terminal/CMD ในโฟลเดอร์โปรเจกต์
3) รัน: npm install
4) รัน: npx cap add android
5) รัน: npx cap sync android
6) รัน: npx cap open android
7) ใน Android Studio เลือก Build > Build Bundle(s) / APK(s) > Build APK(s)
8) APK จะอยู่ใน android/app/build/outputs/apk/debug/

หมายเหตุ:
- ชุดนี้เตรียมโปรเจกต์ Capacitor พร้อม HTML เกม ไม่ใช่ APK ที่คอมไพล์เสร็จแล้ว
- เกมมีการอ้างอิง Google Fonts ผ่านอินเทอร์เน็ต; ส่วนเกมหลักอาจทำงานใน WebView ได้ แต่ฟอนต์อาจใช้ fallback เมื่อ offline
