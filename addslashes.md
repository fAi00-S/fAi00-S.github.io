<h1>addslashs() function</h1><br>
<br><img src="head1.jpg"  width="1069" height="360">
<br>ฟังก์ชัน addslashes() ใน PHP เป็นฟังก์ชันที่ใช้จัดรูปแบบข้อความใหม่โดยการเพิ่ม backslash (\) ข้างหน้าตัวอักษรดังนี้ <br>
<br>- single quote(‘) 
<br>- double quote(“)
<br>- backslashes(\) 
<br>- NULL<br>
<br>เพื่อป้องกันความผิดพลาดหรือป้องกันการใช้งานผิดวัตถุประสงค์จากผู้ไม่ประสงค์ดี <br>
<h2><br>ทำไมต้องใช้ฟังก์ชัน addslashes()</h2>
<br>PHP มีฟังก์ชันพิเศษคือ ฟังก์ชัน addslashes() สำหรับจัดรูปแบบตัวอักษรใหม่ ก่อนการเขียนลง database 
<br>เพื่อป้องกันการเกิด SQL Injection โดย SQL Injection คือการใช้คำสั่งหรือแฝงคำสั่ง SQL จากการรับค่าของผู้ใช้ไปทำการ  query, insert, update, delete หรืออื่นๆ บน Database 
<br>ตัวอย่างของ SQL Injection เช่นมีการรับค่า input จากผู้ใช้งานเป็น username และ password เพื่อ Login ระบบ


<br>$sql = "SELECT username FROM Users where username='$username' AND password='$password';"
<br>$result = $conn->query($sql);
