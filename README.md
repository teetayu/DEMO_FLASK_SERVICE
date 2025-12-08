# DEMO_FLASK_SERVICE  
### รายงานสรุปผลการทดลองสร้าง Web Service ด้วย Flask  

---

##  บทนำ (Introduction)

โปรเจกต์นี้เป็นงานที่อาจารย์มอบหมายเพื่อให้ทดลองสร้าง **Web Service พื้นฐานด้วย Flask Framework**  
โดยมีเป้าหมายเพื่อทำความเข้าใจการทำงานของ Backend เบื้องต้น เช่น การสร้าง API, การรับ–ส่งข้อมูลแบบ JSON,  
การทำงานของ Web Server และการจัดโครงสร้างโปรเจกต์ให้สามารถพัฒนาต่อได้ในอนาคต

โค้ดชุดนี้จึงทำหน้าที่เป็น **Demo Service** เพื่อเรียนรู้ก่อนเข้าสู่ระบบที่ซับซ้อนกว่า เช่น การต่อฐานข้อมูล,  
การสร้าง Machine Learning API, หรือการทำระบบ Authentication

---

##  วัตถุประสงค์ของงาน (Project Objectives)

โปรเจกต์นี้มีเป้าหมายหลักดังนี้:

- ฝึกการใช้งาน Flask ในการสร้าง REST API  
- เรียนรู้การจัดการโครงสร้างไฟล์ในโปรเจกต์ Backend  
- ทดลองสร้าง endpoint แบบง่าย เช่น root path และ status check  
- ใช้ Git และ GitHub สำหรับเก็บโค้ดและจัดการเวอร์ชัน  
- สรุปผลและเขียนรายงานสิ่งที่ได้เรียนรู้จากการทำโปรเจกต์นี้

---

##  โครงสร้างโปรเจกต์ (Project Structure)

```

DEMO_FLASK_SERVICE/
│
├── app.py                 # ไฟล์หลักของ Flask และ Routing
├── requirements.txt        # รายการ dependencies
├── service/                # โฟลเดอร์เก็บ business logic
    └── example_service.py  # ตัวอย่าง service logic

```

การแยกโครงสร้างไฟล์แบบนี้ช่วยให้โค้ดอ่านง่าย, แก้ไขง่าย และสามารถขยายฟีเจอร์ได้ในอนาคต

---

##  เครื่องมือและเทคโนโลยีที่ใช้ (Tools & Technologies Used)

| หมวด | รายละเอียด |
|------|-------------|
| Programming | Python 3 |
| Framework | Flask |
| Libraries | Flask, JSON, Virtual Environment |
| Version Control | Git, GitHub |
| Development Tools | VS Code, Postman |

---

##  วิธีติดตั้งและรันโปรเจกต์ (Setup & Run)

### 1️ Clone โปรเจกต์
```

git clone [https://github.com/teetayu/DEMO_FLASK_SERVICE](https://github.com/teetayu/DEMO_FLASK_SERVICE)

```

### 2️ เข้าโฟลเดอร์โปรเจกต์
```

cd DEMO_FLASK_SERVICE

```

### 3️ สร้าง Virtual Environment
```

python -m venv venv
venv\Scripts\activate   # Windows

```

### 4️ ติดตั้ง Dependencies
```

pip install -r requirements.txt

```

### 5️ รัน Flask Server
```

python app.py

````

API จะเปิดที่  
`http://127.0.0.1:5000/`

---

##  API ที่สร้างในโปรเจกต์นี้ (Example Endpoints)

###  GET `/`
ทดสอบว่าเซิร์ฟเวอร์ทำงานหรือไม่

**Response**
```json
{
  "message": "Flask Service Running"
}
````

---

###  GET `/status`

ส่งสถานะของระบบและข้อความตอบกลับ

**Response**

```json
{
  "status": "OK",
  "service": "Demo Flask API"
}
```

---

##  สิ่งที่ได้ทำในโปรเจกต์นี้ (Summary of Work Done)

งานนี้ครอบคลุมสิ่งที่อาจารย์ต้องการให้ฝึก ดังนี้:

###  การสร้าง Flask Application

* สร้างเซิร์ฟเวอร์ด้วย `Flask(__name__)`
* รัน Web Server ภายในเครื่อง

###  การสร้าง Routing

* กำหนดเส้นทาง API หลายแบบ
* ทดสอบด้วย Browser และ Postman

###  การแยกโครงสร้างโค้ด

* ย้าย logic ไปไว้ใน `service/example_service.py`
* เพิ่มความสามารถในการขยายโปรเจกต์ในอนาคต

###  การใช้งาน JSON Response

* ส่งข้อมูลกลับอย่างเป็นระบบ
* เข้าใจการทำงานของ REST API มากขึ้น

###  การใช้ Git/GitHub

* clone / commit / push / pull
* จัดเก็บงานให้อยู่ใน repository แบบมืออาชีพ

---

##  สิ่งที่ได้เรียนรู้ (What I Learned)

โปรเจกต์นี้ช่วยให้เข้าใจพื้นฐานหลายอย่างของงาน Backend และ DevOps ได้แก่:

###  1) ความเข้าใจ Flask Framework

* วิธีใช้งาน Routing
* การสร้าง Response
* การจัดการโครงสร้างไฟล์

###  2) ความเข้าใจ REST API

* วิธีการรับ–ส่งข้อมูลแบบ JSON
* หลักการออกแบบ endpoint

###  3) ทักษะ Git & GitHub

* การ push โค้ดขึ้น GitHub
* การใช้ repository เพื่อเก็บงานอย่างเป็นระบบ
* ความสำคัญของ README ในโปรเจกต์จริง

###  4) การพัฒนาในสภาพแวดล้อมจริง (Development Workflow)

* การใช้ virtual environment
* การติดตั้ง dependencies
* การรันระบบผ่าน Terminal

---

##  บทสรุป (Conclusion)

โปรเจกต์ DEMO_FLASK_SERVICE เป็นการทดลองสร้างระบบ API ที่เรียบง่าย
แต่มีประโยชน์อย่างมากในแง่การเรียนรู้
