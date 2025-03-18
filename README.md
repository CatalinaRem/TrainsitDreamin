# TransitDreamin
---
แบบภาษาไทยอยู่ข้างล่างนะ
## 🌎 English Version

**TransitDreamin** is an **SQL Database API** designed to provide bus route information in Thailand, focusing on retrieving data from **starting points (bus depots as the primary source)** to help users plan their journeys efficiently.

### 🔹 Key Features
- 🚌 **Provides bus route information for Thailand**
- 📍 **Focuses on data from starting points (bus depots)**
- 📖 **Supports route searches by bus line, stops, and destinations**
- 📡 **Can be used as an API for other applications**
- 🔧 **Designed with SQL to support future scalability**

### 🛠 Installation and Usage

#### 1️⃣ Install Dependencies
```sh
pip install mysql-connector-python
```

#### 2️⃣ Start Using the API
```python
import mysql.connector

def connect_db():
    return mysql.connector.connect(
        host="localhost",
        user="your_user",
        password="your_password",
        database="transitdreamin"
    )

def get_routes():
    db = connect_db()
    cursor = db.cursor(dictionary=True)
    cursor.execute("SELECT * FROM bus_routes")
    return cursor.fetchall()

print(get_routes())
```

### 🚀 Future Development Plans
- [ ] Design and create an ER Diagram
- [ ] Expand bus route data coverage
- [ ] Develop a REST API for route information retrieval
- [ ] Implement advanced route search functionalities
- [ ] Integrate with **Mochiko**, the Discord Bot, to provide cosplay event and travel alerts

### 💡 Frequently Asked Questions (FAQ)
#### ❓ Does TransitDreamin cover all bus routes?
Currently, **not all routes are included**, but plans are in place to expand coverage.

#### ❓ Can TransitDreamin be used in other applications?
Yes! TransitDreamin is designed as an **SQL Database API**, allowing integration with various applications and systems.

#### ❓ Is there an available API?
It is under development, and a RESTful API is expected to be available in the future 🎯

### 👨‍💻 Developer
- **Catalina Rem** - Founder & Developer

### 📜 License
TransitDreamin © 2025 CatalinaRem. All rights reserved.

--

## 🌍 ภาษาไทย

**TransitDreamin** เป็น **SQL Database API** สำหรับการให้ข้อมูลเส้นทางรถเมล์ในประเทศไทย โดยเน้นการดึงข้อมูลจาก **ต้นทาง (อู่รถเมล์เป็นหลัก)** เพื่อช่วยให้ผู้ใช้สามารถวางแผนการเดินทางได้อย่างสะดวกยิ่งขึ้น

### 🔹 คุณสมบัติเด่น
- 🚌 **ให้ข้อมูลเส้นทางรถเมล์ในประเทศไทย** 
- 📍 **เน้นข้อมูลจากต้นทาง (อู่รถเมล์เป็นหลัก)**
- 📖 **รองรับการค้นหาเส้นทางตามสายรถเมล์, จุดจอด และปลายทาง**
- 📡 **สามารถใช้เป็น API สำหรับแอปพลิเคชันอื่น ๆ ได้**
- 🔧 **ออกแบบด้วย SQL เพื่อรองรับการขยายระบบในอนาคต**

### 🛠 วิธีติดตั้งและใช้งาน

#### 1️⃣ ติดตั้ง Dependencies
```sh
pip install mysql-connector-python
```

#### 2️⃣ เริ่มใช้งาน API
```python
import mysql.connector

def connect_db():
    return mysql.connector.connect(
        host="localhost",
        user="your_user",
        password="your_password",
        database="transitdreamin"
    )

def get_routes():
    db = connect_db()
    cursor = db.cursor(dictionary=True)
    cursor.execute("SELECT * FROM bus_routes")
    return cursor.fetchall()

print(get_routes())
```

### 🚀 แผนพัฒนาในอนาคต
- [ ] ออกแบบและสร้าง ER Diagram
- [ ] เพิ่มข้อมูลเส้นทางรถเมล์ให้ครบถ้วน
- [ ] เพิ่มระบบ API สำหรับเรียกดูข้อมูลเส้นทางผ่าน REST API
- [ ] รองรับฟังก์ชันการค้นหาเส้นทางที่ดีที่สุด
- [ ] ผสานรวมกับ Discord Bot **Mochiko** เพื่อให้บริการแจ้งเตือนงานคอสเพลย์และการเดินทาง

### 💡 คำถามที่พบบ่อย (FAQ)
#### ❓ TransitDreamin รองรับรถเมล์ทุกสายหรือไม่?
ปัจจุบัน **ยังไม่ครบทุกสาย** แต่มีแผนจะขยายข้อมูลให้ครอบคลุมมากขึ้น

#### ❓ สามารถใช้ TransitDreamin ในแอปพลิเคชันอื่นได้ไหม?
ได้! TransitDreamin ออกแบบให้เป็น **SQL Database API** ที่สามารถดึงข้อมูลไปใช้กับแอปพลิเคชันหรือระบบอื่น ๆ ได้

#### ❓ มี API ให้ใช้งานหรือไม่?
อยู่ในระหว่างการพัฒนา คาดว่าจะเปิด API RESTful ให้ใช้งานในอนาคต 🎯

### 👨‍💻 ผู้พัฒนา
- **Catalina Rem** - Founder & Developer

### 📜 ลิขสิทธิ์
TransitDreamin © 2025 CatalinaRem. All rights reserved.
