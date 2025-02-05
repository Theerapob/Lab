# ใบงานการทดลอง HTML

## การทดลองที่ 5: การสร้างตารางและรายการ
### วัตถุประสงค์
- เรียนรู้การสร้างตารางข้อมูล
- เรียนรู้การสร้างรายการแบบต่างๆ

### ขั้นตอนการทดลอง
1. สร้างไฟล์ tablelist.html ดังตัวอย่าง:
```html
<table border="1">
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
        </tr>
    </tbody>
</table>
```

### คำอธิบายเพิ่มเติม
- `<table>` กำหนดขอบเขตของตาราง
- `<thead>` สำหรับส่วนหัวตาราง
- `<tbody>` สำหรับเนื้อหาตาราง
- `<tr>` แทนแถว
- `<th>` แทนเซลล์หัวตาราง
- `<td>` แทนเซลล์ข้อมูล

2. การสร้างรายการ โดยเพิ่มเติม Code ในไฟล์ tablelist.html :
```html
<ul>
    <li>Unordered item 1</li>
    <li>Unordered item 2</li>
</ul>

<ol>
    <li>Ordered item 1</li>
    <li>Ordered item 2</li>
</ol>

<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```

### คำอธิบายเพิ่มเติม
- `<ul>` สำหรับรายการแบบไม่เรียงลำดับ
- `<ol>` สำหรับรายการแบบเรียงลำดับ
- `<dl>` สำหรับรายการแบบคำจำกัดความ
- `<li>` แทนรายการแต่ละรายการ

### แบบฝึกหัด
1. สร้างตารางแสดงข้อมูลส่วนตัว
2. สร้างรายการเมนูอาหาร

[วางโค้ด HTML ที่นี่]
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <title>ข้อมูลส่วนตัวและเมนูอาหาร</title>
    <style>
        table {
            border-collapse: collapse;
            width: 50%;
            margin: 20px auto;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 10px;
            text-align: center;
        }
        ul {
            list-style-type: disc;
            width: 50%;
            margin: 20px auto;
        }
    </style>
</head>
<body>
    <h1 style="text-align: center;">ข้อมูลส่วนตัว</h1>
    <table>
        <tr>
            <th>ชื่อ</th>
            <td>ธีรภพ พรหมวิหาร</td>
        </tr>
        <tr>
            <th>อายุ</th>
            <td>19 ปี</td>
        </tr>
        <tr>
            <th>ที่อยู่</th>
            <td>16 ร่มเกล้า 20 ถนนร่มเกล้า เขตมีนบุรี เเขวงมีนบุรี กรุงเทพฯ</td>
        </tr>
        <tr>
            <th>อีเมล</th>
            <td>pob.trp@gmail.com</td>
        </tr>
    </table>

    <h1 style="text-align: center;">เมนูอาหาร</h1>
    <ul>
        <li>ข้าวผัดกระเพราไก่ไข่ดาว</li>
        <li>ต้มยำกุ้ง</li>
        <li>ส้มตำปูปลาร้า</li>
        <li>ข้าวมันไก่</li>
        <li>ขนมจีนแกงเขียวหวาน</li>
    </ul>
</body>
</html>
[วางภาพ screenshot ที่นี่]
![lab 5](https://github.com/user-attachments/assets/3a044ae7-2c8f-4a0c-92a2-a437fb54923a)
