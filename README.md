# Profile
lol
# 👋 ยินดีต้อนรับสู่ GitHub ของฉัน!

---

## 👤 ข้อมูลส่วนตัว (About Me)

<div align="center">
  <img src="http://110.78.30.115/files/importpicstd/01/69319010008.jpg"/>

  ### [ธัชชัย ชอบธรรม]
  🎯 *นักศึกษาเทคโนโลยีสารสนเทศ | Backend Developer Trainee*
</div>

---

## 🎯 จุดประสงค์ในการเข้าศึกษาต่อ

ฉันมีความตั้งใจและมุ่งมั่นที่จะเข้าศึกษาต่อที่ **วิทยาลัยพณิชยการบางนา สาขาวิชาเทคโนโลยีสารสนเทศ** เนื่องจากเหตุผลดังต่อไปนี้:
* **พัฒนาทักษะเฉพาะทาง:** เพื่อยกระดับความรู้ด้านการเขียนโปรแกรมและการจัดการระบบสารสนเทศให้เป็นระบบและได้มาตรฐานสากล
* **ต่อยอดความหลงใหล:** มีความสนใจอย่างแรงกล้าในการพัฒนา Web Application โดยเฉพาะระบบเบื้องหลัง (Backend)
* **เตรียมพร้อมสู่อาชีพ:** เพื่อเตรียมความพร้อมและสร้างฐานความรู้ที่มั่นคงสำหรับการประกอบอาชีพ Back-end Developer ในอนาคต

---

## 💻 การเรียนในรายวิชา Backend Development

ในการเรียนวิชานี้ ฉันได้ศึกษาเกี่ยวกับการพัฒนาส่วนหลังของระบบ ซึ่งประกอบไปด้วยหัวข้อหลักและหัวข้อย่อยดังนี้:

### 1. Fundamentals of Backend
* ทำความเข้าใจสถาปัตยกรรมแบบ Client-Server
* การทำงานของ HTTP Requests / Responses (GET, POST, PUT, DELETE)
* รู้จักและใช้งาน JSON Data

### 2. Node.js & Runtime Environment
* การติดตั้งและการใช้งาน Node.js
* การบริหารจัดการ Package ด้วย NPM (Node Package Manager)
* การใช้งาน Built-in Modules (เช่น `fs`, `http`, `path`)

### 3. Express.js Framework
* การสร้าง Web Server ด้วย Express
* การทำ Routing (กำหนดเส้นทางของ URL)
* การใช้งาน Middleware เพื่อจัดการข้อมูลก่อนส่งต่อ

### 4. Database Integration
* การเชื่อมต่อฐานข้อมูล (SQL / NoSQL)
* การใช้งานคู่กับ ORM/ODM (เช่น Mongoose, Sequelize)
* การทำ CRUD Operations (Create, Read, Update, Delete)

---

## 📝 ตัวอย่างการเขียน Code ด้วย Node.js (Express.js)

นี่คือตัวอย่างการสร้าง Web API แบบง่ายๆ ด้วย Node.js และ Express framework สำหรับเริ่มต้นระบบ Server:

```javascript
// 1. นำเข้า Express Module
const express = require('express');
const app = express();
const PORT = 3000;

// 2. รองรับการอ่านข้อมูลแบบ JSON
app.use(express.json());

// 3. หัวข้อย่อย: การสร้าง Routing พื้นฐาน
// หน้าแรก (Home Route)
app.get('/', (req, res) => {
    res.send('ยินดีต้อนรับสู่ Backend Server ของฉัน! 🚀');
});

// ดึงข้อมูลตัวอย่าง (Get Data)
app.get('/api/user', (req, res) => {
    res.json({
        id: 1,
        name: "นักศึกษา พณิชยการบางนา",
        major: "Information Technology"
    });
});

// 4. สั่งให้ Server ทำงานที่ Port ที่กำหนด
app.listen(PORT, () => {
    console.log(`Server กำลังรันอยู่ที่ http://localhost:${PORT}`);
});