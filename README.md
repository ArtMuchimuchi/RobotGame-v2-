# สมาชิก

1. นายชิษณุพงศ์ วิภาชัยนันท์ 63090500407

2. นายปรมัตถ์ วงษ์ผึ่ง 63090500413

3. นายชิณกฤต บันลือปัญญาดี 63090500422

4. นางสาวภัทรวริน เจียมทอง 63090500430

5. นายธนธัช เลิศพินิจอมรกุล 63090500438

6. นายวรบดินทร์ เปี่ยมมหามงคล 63090500441

---

# Robot Game

---

### คำอธิบายไฟล์

หลักการทำงานของโปรแกรม **Robot Game** จะมีลักษณะเป็นแบบ **Client-Server**

โดยที่ทางฝั่งของ **Server** จะมีหน้าที่รับผิดชอบในการสร้างแผนที่ส่วนกลาง

หรือการคำนวนต่างๆที่ต้องมีการบันทึกลงแผนที่ ซึ่งทาง **Server** จะคอยรับ

**Message** ที่ส่งมาจาก **Client** เพื่อรับคำสั่งแล้วประมวลผล (โดยคำสั่งที่มี

การยุ่งเกี่ยวกับแผนที่ส่วนกลางจะมีการใช้ **Synchronize** เพื่อป้องกันข้อผิดพลาด

ในการอัพเดทแผนที่) จากนั้นจะทำการอัพเดทแผนที่ส่วนกลาง แล้วทำการส่งแผนที่

ดังกล่าวในรูปแบบ **Object** ผ่าน **Socket** ไปยัง **Client** 


ในฝั่งของ **Client** นั้นจะรับผิดชอบในการรับข้อมูล **object** แผนที่ที่มากจากฝั่ง

**Server** แล้วนำไปแสดงผล และยังมีหน้าที่รับคำสั่งการควบคุมจาก **User** ส่งเป็น **Message**

กลับไปยัง **Server**

---

# การรันโปรแกรมฝั่ง Server

1.เปิด command prompt แล้วทำการ cd มาที่ folder robotGame (ไม่ใช่ RobotGame-v2-)

![picture1](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture1.jpg)

2. พิมคำสั่ง java Server เพื่อทำการเปิด Server

![picture2](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture2.jpg)

# การรันโปรแกรมฝั่ง Client 
1.ต้องทำการเปิด Server ก่อน

2.เปิด command prompt แล้วทำการ cd มาที่ folder robotGame (ไม่ใช่ RobotGame-v2-)

![picture1](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture1.jpg)

3.พิมคำสั่ง java robotGame จะมีหน้าต่างใหม่ขึ้นมา ให้ทำการกรอกชื่อผู้เล่นและกด submit

![picture3](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture3.jpg)

![picture4](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture4.jpg)

4.เมื่อกด submit จะมีหน้าต่างของตัวเกมขึ้นมา สามารถเคลื่อนที่ด้วยปุ่มลูกศร และยิงได้ด้วยปุ่ม spacebar

![picture5](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture5.jpg)

5.หากต้องการเพิ่มผู้เล่นใหม่ (สูงสุด 4 ผู้เล่น) ให้ทำตามข้อ 2, 3 อีกครั้ง

---

## ข้อมูลเพิ่มเติม

1.เกมจะจบเมื่อมีผู้เล่นคนใดคนนึงมีเลือดเท่ากับหรือต่ำกว่า 0 

2.เมื่อเกมจบจะมีหน้าต่างใหม่ขึ้นมาสำหรับแต่ละผู้เล่น โดยผู้เล่นที่เลือดเท่ากับหรือต่ำกว่า 0 จะถือว่าแพ้ ส่วนคนที่เหลือจะนับว่าชนะ

![picture6](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture6.jpg)

![picture7](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture7.jpg)

3.เมื่อเกมจบแล้ว command prompt ของ Server อาจจะค้างอยู่ ให้ทำการกด ctrl+c เพื่อให้กลับมาพิมคำสั่งได้

![picture8](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture8.jpg)

![picture9](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture9.jpg)

4.หากออกเกมด้วยวิธีอื่นที่ไม่ใช่การจบเกมปกติ command prompt ของ server หรือ client อาจค้างได้ ให้แก้ด้วยวิธีเดียวกันกับข้อ 3

![picture10](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture10.jpg)

![picture11](https://github.com/ArtMuchimuchi/RobotGame-v2-/blob/main/others/picture11.jpg)

