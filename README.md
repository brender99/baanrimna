# baanrimna

## คำสั่ง Git สำหรับการ Push โค้ด

### การเริ่มต้นโปรเจค (ทำครั้งแรกเท่านั้น)
```
git init
git branch -M main
git remote add origin https://github.com/brender99/baanrimna.git
```

### คำสั่งที่ใช้ทุกครั้งที่ต้องการ Push โค้ด

```
# ตรวจสอบสถานะไฟล์ที่มีการเปลี่ยนแปลง
git status

# เพิ่มไฟล์ที่ต้องการ commit
git add .              # เพิ่มทุกไฟล์ที่มีการเปลี่ยนแปลง
git add <ชื่อไฟล์>      # เพิ่มเฉพาะไฟล์ที่ระบุ

# บันทึกการเปลี่ยนแปลง (Commit)
git commit -m "ข้อความอธิบายการเปลี่ยนแปลง"

# อัปโหลดโค้ดไปยัง GitHub
git push -u origin main
```

### คำสั่งอื่นๆ ที่มีประโยชน์

```
# ดูประวัติการ commit
git log

# ดึงโค้ดล่าสุดจาก GitHub
git pull

# สร้างและสลับไปยัง branch ใหม่
git checkout -b <ชื่อ-branch-ใหม่>

# สลับไปยัง branch อื่น
git checkout <ชื่อ-branch>

# รวม branch
git merge <ชื่อ-branch-ที่ต้องการรวม>
```

## ประวัติการเริ่มต้นโปรเจค

PS D:\www\baanrimna> echo "# baanrimna" >> README.md
PS D:\www\baanrimna> git init
Initialized empty Git repository in D:/www/baanrimna/.git/
PS D:\www\baanrimna> git add README.md
PS D:\www\baanrimna> git commit -m "first commit"
[master (root-commit) c5ca2f6] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
PS D:\www\baanrimna> git branch -M main
PS D:\www\baanrimna> git remote add origin https://github.com/brender99/baanrimna.git
PS D:\www\baanrimna> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 251 bytes | 251.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/brender99/baanrimna.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.