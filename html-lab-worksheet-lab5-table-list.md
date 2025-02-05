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
    <title>แสดงโค้ด HTML</title>
</head>
<body>
    <h1>แสดงโค้ด HTML</h1>
    <pre><code>
&lt;!DOCTYPE html&gt;
&lt;html lang="th"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;title&gt;ข้อมูลส่วนตัวและเมนูอาหาร&lt;/title&gt;
    &lt;style&gt;
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
    &lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;h1 style="text-align: center;"&gt;ข้อมูลส่วนตัว&lt;/h1&gt;
    &lt;table&gt;
        &lt;tr&gt;
            &lt;th&gt;ชื่อ&lt;/th&gt;
            &lt;td&gt;ธีรภพ พรหมวิหาร&lt;/td&gt;
        &lt;/tr&gt;
        &lt;tr&gt;
            &lt;th&gt;อายุ&lt;/th&gt;
            &lt;td&gt;19 ปี&lt;/td&gt;
        &lt;/tr&gt;
        &lt;tr&gt;
            &lt;th&gt;ที่อยู่&lt;/th&gt;
            &lt;td&gt;16 ร่มเกล้า 20 ถนนร่มเกล้า เขตมีนบุรี เเขวงมีนบุรี กรุงเทพฯ&lt;/td&gt;
        &lt;/tr&gt;
        &lt;tr&gt;
            &lt;th&gt;อีเมล&lt;/th&gt;
            &lt;td&gt;pob.trp@gmail.com&lt;/td&gt;
        &lt;/tr&gt;
    &lt;/table&gt;

    &lt;h1 style="text-align: center;"&gt;เมนูอาหาร&lt;/h1&gt;
    &lt;ul&gt;
        &lt;li&gt;ข้าวผัดกระเพราไก่ไข่ดาว&lt;/li&gt;
        &lt;li&gt;ต้มยำกุ้ง&lt;/li&gt;
        &lt;li&gt;ส้มตำปูปลาร้า&lt;/li&gt;
        &lt;li&gt;ข้าวมันไก่&lt;/li&gt;
        &lt;li&gt;ขนมจีนแกงเขียวหวาน&lt;/li&gt;
    &lt;/ul&gt;
    
&lt;/body&gt;
&lt;/html&gt;
    </code></pre>
</body>
</html>

[วางภาพ screenshot ที่นี่]
![lab 5](https://github.com/user-attachments/assets/ffb0e1c6-349e-4ff4-b9b0-f71528ffea52)


