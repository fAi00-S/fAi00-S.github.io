#addslashs() function
![](img src="head1.jpg"  width="1069" height="360")
ฟังก์ชัน addslashes() ใน PHP เป็นฟังก์ชันที่ใช้จัดรูปแบบข้อความใหม่โดยการเพิ่ม backslash (\) ข้างหน้าตัวอักษรดังนี้
- single quote(‘) 
- double quote(“)
- backslashes(\) 
- NULL<br>
เพื่อป้องกันความผิดพลาดหรือป้องกันการใช้งานผิดวัตถุประสงค์จากผู้ไม่ประสงค์ดี
##ทำไมต้องใช้ฟังก์ชัน addslashes()
SQL Injection คือการใช้คำสั่งหรือแฝงคำสั่ง SQL จากการรับค่าจากผู้ใช้ไปทำการ  query, insert, update, delete หรืออื่นๆ บน Database 
โดย PHP มีฟังก์ชันพิเศษคือ ฟังก์ชัน addslashes() สำหรับจัดรูปแบบตัวอักษรใหม่ ก่อนการเขียนลง database เช่นมีการรับค่า username และ password ในระบบงานหนึ่ง
