# V23 Mobile App Shell — แอปคิวงาน เติมรัก

แพ็กเกจนี้เป็น PWA shell สำหรับเปิด Google Apps Script Web App แบบ standalone โดยใช้ iframe ภายใน shell เพื่อซ่อน URL bar ของ Chrome

## ไฟล์
- index.html — ตัว shell
- manifest.webmanifest — กำหนดชื่อ/ไอคอน/standalone
- service-worker.js — cache ของ shell
- icon-192.png / icon-512.png — ไอคอน

## สำคัญ
ต้องนำไฟล์ชุดนี้ไปโฮสต์บน HTTPS static hosting (เช่น GitHub Pages/Cloudflare Pages/Netlify) ก่อน จึงจะติดตั้งเป็น PWA ได้จริง

Google Apps Script V23 ปัจจุบันมี XFrameOptionsMode.ALLOWALL อยู่แล้ว จึงสามารถถูกฝังใน shell ได้
