<h1>addslashs() function</h1><br>
<br><img src="head1.jpg"  width="1069" height="360">
<br>ฟังก์ชัน addslashes() ใน PHP เป็นฟังก์ชันที่ใช้จัดรูปแบบข้อความใหม่โดยการเพิ่ม backslash (\) ข้างหน้าตัวอักษรดังนี้ <br>
<br>- single quote(‘) 
<br>- double quote(“)
<br>- backslashes(\) 
<br>- NULL<br>
<br>เพื่อป้องกันความผิดพลาดหรือป้องกันการใช้งานผิดวัตถุประสงค์จากผู้ไม่ประสงค์ดี <br>
<h2><br>ทำไมต้องใช้ฟังก์ชัน addslashes()</h2>
<br>SQL Injection คือการใช้คำสั่งหรือแฝงคำสั่ง SQL จากการรับค่าจากผู้ใช้ไปทำการ  query, insert, update, delete หรืออื่นๆ บน Database 
<br>โดย PHP มีฟังก์ชันพิเศษคือ ฟังก์ชัน addslashes() สำหรับจัดรูปแบบตัวอักษรใหม่ ก่อนการเขียนลง database เช่นมีการรับค่า username และ password ในระบบงานหนึ่ง
