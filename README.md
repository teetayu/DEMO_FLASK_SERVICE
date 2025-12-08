# DEMO_FLASK_SERVICE  
### รายงานสรุปการทดลองสร้าง Web Service ด้วย Flask  

---

##  บทนำ (Introduction)

งานนี้เป็นแบบฝึกหัดเพื่อทดลองสร้าง **Web Service แบบง่าย ๆ ด้วย Flask Framework**  
โดยอาจารย์ให้โจทย์ให้ลองออกแบบ API พื้นฐานขึ้นมา 1 โปรเจกต์ เพื่อให้เข้าใจหลักการของ Backend  
ตั้งแต่การรันเซิร์ฟเวอร์, การสร้าง Route, การคืนค่า Response, จนถึงการจัดโครงสร้างโปรแกรมให้ถูกต้อง

โปรเจกต์นี้จึงถือเป็นการปูพื้นฐานก่อนที่จะทำระบบที่มีความซับซ้อนมากขึ้น เช่น  
API สำหรับ Machine Learning, ระบบ Database หรือระบบ Authentication

---

##  สิ่งที่โปรเจกต์นี้ทำ (What This Project Does)

โปรเจกต์นี้เป็น **ตัวอย่างบริการ Flask แบบง่าย ๆ (Demo Service)**  
ประกอบด้วย:

- การสร้าง Web Server ด้วย Flask  
- การกำหนดเส้นทาง (Route) เช่น `/` หรือ `/status`  
- ส่งข้อมูลกลับเป็น JSON Response  
- แยกโค้ดเป็นไฟล์เพื่อให้อ่านง่ายและแก้ไขได้สะดวก  

ตัวอย่างที่ทำได้ เช่น:

- ตรวจสอบสถานะของระบบผ่าน `/status`  
- ส่งข้อความหรือข้อมูลทดสอบกลับไปยังผู้เรียกใช้ API  
- ใช้เป็นพื้นฐานสำหรับต่อยอด API อื่น ๆ

---

##  โครงสร้างโปรเจกต์ (Project Structure)

DEMO_FLASK_SERVICE/
│
├── app.py # ไฟล์หลักของ Flask
├── requirements.txt # รายการ library ที่ใช้
├── service/ # ตัวอย่างแยก logic ออกมาจาก app.py
│ └── example_service.py

---

##  วิธีการรันโปรเจกต์ (How to Run)

1. **Clone โปรเจกต์**
git clone https://github.com/teetayu/DEMO_FLASK_SERVICE


2. **เข้าโฟลเดอร์โปรเจกต์**
cd DEMO_FLASK_SERVICE


3. **สร้าง Virtual Environment (แนะนำ)**
python -m venv venv
venv\Scripts\activate # Windows


4. **ติดตั้ง Library**
pip install -r requirements.txt


5. **รัน Flask**
python app.py


เมื่อเซิร์ฟเวอร์รันสำเร็จ สามารถเข้าที่  
`http://127.0.0.1:5000/`

---

##  ตัวอย่าง API ที่ทำ

### GET `/`
ส่งข้อความตอบกลับว่าระบบทำงานอยู่

### GET `/status`
ส่งสถานะของระบบ เช่น

```json
{
  "status": "OK",
  "service": "Demo Flask API"
}

---

 สรุปสิ่งที่ได้ทำในงานนี้ (Summary of Work Done)

ในงานนี้ได้ทำสิ่งสำคัญดังนี้:

ติดตั้งและตั้งค่า Flask Framework

สร้าง Web Server ที่รันบน Localhost

ทำ Routing แบบง่าย เช่น / และ /status

สร้าง Response แบบ JSON

แยก Business Logic ออกไปไว้ในโฟลเดอร์ service/

ทดสอบ API ผ่าน Browser หรือ Postman

อัปโหลดโปรเจกต์ขึ้น GitHub

ใช้ Git ในการ push และจัดการเวอร์ชันของโค้ด

ทำเอกสาร README เพื่อสรุปงานให้ผู้อ่านเข้าใจโครงสร้างโปรเจกต์

 สิ่งที่ได้เรียนรู้จากโปรเจกต์นี้ (What I Learned)

งานนี้ช่วยให้เข้าใจหลักการพื้นฐานของ Backend และการสร้าง Web API ได้แก่:

 1) ความเข้าใจ Flask มากขึ้น

วิธีสร้าง API ด้วย Python

การกำหนด Route และ Response

การจัดโครงสร้างโปรแกรมให้ขยายได้ง่ายขึ้น

 2) การทำงานของ REST API

วิธีรับ–ส่งข้อมูลระหว่าง Client และ Server

ความสำคัญของ JSON Response

 3) การใช้งาน Git & GitHub ในโปรเจกต์จริง

การ commit, push, pull

การเก็บโปรเจกต์ใน Repository จริง

ความสำคัญของ README ในการสรุปงาน

 4) ทักษะการจัดระเบียบโค้ด

แยก service ออกจาก app

ทำให้โค้ดอ่านง่ายและแก้ไขได้ในอนาคต

 สรุปผลการทำงาน (Conclusion)

โปรเจกต์นี้ช่วยให้เข้าใจพื้นฐานของการสร้าง Web Service ด้วย Flask
รวมถึงการใช้งาน Git/GitHub ในการจัดการโปรเจกต์
