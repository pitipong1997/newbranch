Git branch

git branch Dev เป็นคำสั่งที่ใช้ในแสดงและแตงกิ่งสาขาในการพัฒนา ซึ่งทำให้การพัฒนาซอฟต์แวร์มีความยืดยุ่นมากขึ้น

สร้าง branch ชื่อ Dev git branch feature

สร้าง branch ชื่อ feature

git checkout Dev เป็นคำสั่งที่ใช้ในการสลับ Working Directory ไปยัง Branch หรือ Commit ที่เราระบุ คำสั่งนี้ยังสามารถให้งานได้ในอีกหลายๆ แบบ ย้ายการทำงานไปที่ Branch หรือ commit_id ที่ระบุ git add . เป็นคำสั่งที่ใช้เพิ่มการเปลี่ยนแปลงของ Source Code เข้าไปที่สถานะ Staged ใช้ในกรณีที่มีหลายๆ ไฟล์และต้องการเพิ่มเข้าไปทั้งหมด

git commmit -m Add Dev.md เป็นคำสั่งที่ใช้ยืนยัน Source Code ที่อยู่ในสถานะ Staged เข้าไปเก็บไว้ที่ Local Repository ยืนยันการเปลี่ยนแปลงพร้อมข้อความ

git push -u origin Dev ทำการส่งการเปลี่ยนแปลงเหล่านี้ ไปยัง remote repository สามารถทำการเปลี่ยน master เป็นชื่อ branch ที่คุณต้องการได้ โดยชื่อที่ใช้เป็น Dev เป็นคำสั่งที่ใช้ยืนยัน Source Code ที่อยู่ในสถานะ Staged เข้าไปเก็บไว้ที่ Local Repository ยืนยันการเปลี่ยนแปลงพร้อมข้อความ

git merge --no-ff Dev เป็นคำสั่งที่ใช้ในการรวม Branch หรือ Commit ทั้งสองเข้าด้วยกัน

git push เป็นคำสั่งที่ใช้ส่งการเปลี่ยนแปลงของ Source Code ที่เก็บอยู่บน Local Repository ขึ้นไปยัง Remote Repository

git fetch เป็นคำสั่งที่ใช้รับการเปลี่ยนแปลงของ Source Code ล่าสุดที่อยู่บน Remote Repository ลงมายัง Local Repository แต่ยังไม่ได้ทำการรวม Source Code (Merge)

git pull origin master เป็นคำสั่งที่ใช้รับการเปลี่ยนแปลงของ Source Code ล่าสุดที่อยู่บน Remote Repository ลงมายัง Local Repository และทำการ Auto Merge

git clone เป็นคำสั่งที่ใช้ดึงประวัติทั้งหมดบน Remote Repository ของเพื่อนร่วมทีม ของคนอื่นหรือของเราเองที่มีอยู่แล้วบน Git Hosting มาที่เครื่องของเรา คำสั่งนี้จะคล้ายๆ Git Init ที่ใช้สร้างระบบ Git ขึ้นมาตอนเริ่มต้น แต่เราจะได้ประวัติเดิมของ Repository มาด้วย ทำให้เราเริ่มพัฒนาต่อจากตรงจุดนี้ได้เลย

git stash เป็นคำสั่งที่ใช้ซ่อนการเปลี่ยนแปลงใน Working Directory ทำให้ Working Directory Clean นิยมใช้ก่อนคำสั่ง Git Pull