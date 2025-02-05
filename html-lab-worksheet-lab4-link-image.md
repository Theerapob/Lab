# ใบงานการทดลอง HTML

## การทดลองที่ 4: การสร้างลิงก์และการแทรกรูปภาพ

### การเตรียมโครงสร้างโฟลเดอร์และไฟล์
1. สร้างโครงสร้างโฟลเดอร์:
   ```
   html-workshop/
   ├── index.html
   ├── pages/
   │   ├── about.html
   │   └── contact.html
   ├── images/
   │   ├── logo.jpg
   │   └── products/
   │       ├── product1.jpg
   │       └── product2.jpg
   └── files/
       └── document.pdf
   ```

2. ขั้นตอนการสร้างโครงสร้าง:
   - คลิกขวาในโฟลเดอร์ html-workshop > New Folder > สร้าง "pages"
   - คลิกขวาในโฟลเดอร์ html-workshop > New Folder > สร้าง "images"
   - ในโฟลเดอร์ images > New Folder > สร้าง "products"
   - คลิกขวาในโฟลเดอร์ html-workshop > New Folder > สร้าง "files"

3. สร้างไฟล์ HTML:
   - ในโฟลเดอร์หลัก: สร้าง index.html (ใช้ไฟล์เดิมที่มีได้)
   - ในโฟลเดอร์ pages: สร้าง about.html และ contact.html

4. จัดเตรียมไฟล์:
   - นำรูปภาพที่ต้องการใช้ไปไว้ในโฟลเดอร์ images
   - นำรูปภาพสินค้าไปไว้ในโฟลเดอร์ products
   - นำไฟล์เอกสารไปไว้ในโฟลเดอร์ files

### ขั้นตอนการทดลอง

#### ส่วนที่ 1: การสร้างลิงก์
1. เปิดไฟล์ index.html และใส่โครงสร้างพื้นฐาน:
```html
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <title>หน้าหลัก</title>
</head>
<body>
    <!-- ส่วนของเนื้อหา -->
</body>
</html>
```

2. สร้างเมนูนำทางพื้นฐาน:
```html
<nav>
    <!-- ลิงก์ภายใน - ไปยังหน้าในเว็บไซต์เดียวกัน -->
    <a href="index.html">หน้าหลัก</a>
    <a href="pages/about.html">เกี่ยวกับเรา</a>
    <a href="pages/contact.html">ติดต่อเรา</a>
    
    <!-- ลิงก์ภายนอก - เปิดในแท็บใหม่ -->
    <a href="https://www.google.com" target="_blank">
        ไปยัง Google
    </a>
</nav>
```
คำอธิบาย:
- `href="..."` - กำหนดเส้นทางของลิงก์
- `target="_blank"` - เปิดลิงก์ในแท็บใหม่

3. สร้างลิงก์ภายในหน้าเดียวกัน:
```html
<!-- สร้างจุดเชื่อมโยง -->
<section id="top">
    <h1>เนื้อหาส่วนบน</h1>
</section>

<section id="products">
    <h2>สินค้าของเรา</h2>
</section>

<!-- ลิงก์ไปยังจุดเชื่อมโยง -->
<a href="#top">กลับด้านบน</a>
<a href="#products">ไปยังสินค้า</a>
```
คำอธิบาย:
- `id="..."` - กำหนดจุดเชื่อมโยง
- `href="#..."` - ลิงก์ไปยัง id ที่กำหนด

4. สร้างลิงก์พิเศษ:
```html
<!-- ลิงก์อีเมล -->
<a href="mailto:contact@example.com">ส่งอีเมลหาเรา</a>

<!-- ลิงก์โทรศัพท์ -->
<a href="tel:+66812345678">โทร 081-234-5678</a>

<!-- ลิงก์ดาวน์โหลด -->
<a href="files/document.pdf" download>
    ดาวน์โหลดเอกสาร
</a>
```
คำอธิบาย:
- `mailto:` - เปิดโปรแกรมอีเมล
- `tel:` - เปิดโปรแกรมโทรศัพท์
- `download` - ดาวน์โหลดไฟล์แทนการเปิด

#### ส่วนที่ 2: การแทรกรูปภาพ
1. แทรกรูปภาพพื้นฐาน:
```html
<!-- รูปภาพในโฟลเดอร์ images -->
<img src="images/logo.jpg" 
     alt="โลโก้บริษัท"
     width="200">

<!-- รูปภาพในโฟลเดอร์ย่อย products -->
<img src="images/products/product1.jpg" 
     alt="สินค้าชิ้นที่ 1"
     width="300"
     height="200">
```
คำอธิบาย:
- `src="..."` - ระบุตำแหน่งของรูปภาพ
- `alt="..."` - ข้อความทดแทนเมื่อไม่สามารถแสดงรูปได้
- `width="..."` - กำหนดความกว้าง
- `height="..."` - กำหนดความสูง

2. ใช้ figure และ figcaption:
```html
<figure>
    <img src="images/products/product2.jpg" 
         alt="สินค้าชิ้นที่ 2">
    <figcaption>
        รายละเอียดสินค้าชิ้นที่ 2
    </figcaption>
</figure>
```
คำอธิบาย:
- `<figure>` - จัดกลุ่มรูปภาพและคำอธิบาย
- `<figcaption>` - คำอธิบายประกอบรูปภาพ

3. สร้างรูปภาพที่คลิกได้:
```html
<a href="images/products/product1.jpg">
    <img src="images/products/product1.jpg" 
         alt="คลิกเพื่อดูรูปขนาดใหญ่"
         width="200">
</a>
```

### หมายเหตุ
- ตรวจสอบการสะกดชื่อไฟล์และโฟลเดอร์ให้ถูกต้อง
- path ของรูปภาพต้องถูกต้องตามโครงสร้างโฟลเดอร์
- ทดสอบการทำงานของลิงก์ทุกจุด

### แบบฝึกหัด
1. สร้างแกลเลอรีสินค้า:
   - สร้างโฟลเดอร์ images/gallery
   - ใส่รูปภาพอย่างน้อย 4 รูป
   - แต่ละรูปต้องคลิกดูขนาดใหญ่ได้
   - มีคำอธิบายใต้รูป
   - มีปุ่มกลับด้านบน

### บันทึกผลการทดลอง
- รหัสเอกสาร HTML ที่เขียน:
```html
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <title>หน้าหลัก</title>
    <style>
        .center {
            text-align: center;
            margin-bottom: 20px;
        }
        .center-img {
            display: flex;
            justify-content: center;
            align-items: center;
        }
    </style>
</head>
<body>
    <h1 class="center">ยินดีต้อนรับสู่ร้านขายสินค้า Hololive</h1>
    
    <div class="center-img">
        <img src="https://hololivepro.com/wp-content/uploads/2023/03/hololive_hp.png" alt="logo" width="300">
    </div>
    <style>
        nav {
            text-align: center;
            margin: 20px 0;
        }
    </style>
    <nav>
        <a href="index.html">หน้าหลัก</a>
        <a href="pages/about.html">เกี่ยวกับเรา</a>
        <a href="pages/contact.html">ติดต่อเรา</a>
        <a href="https://shop.hololivepro.com/" target="_blank">ไปยังหน้าสินค้า Official</a>
    </nav>

    <section id="top">
        <h1>ประวัติ Hololive</h1>
        <p>คัฟเวอร์คอร์โปเรชัน (ญี่ปุ่น: カバー株式会社; โรมาจิ: Kabā Kabushiki-gaisha) ถูกจัดตั้งขึ้นเมื่อวันที่ 13 มิถุนายน ค.ศ. 2016 โดย โมโตอากิ ทานิโงะ (ยาโกะ) ผู้ที่เคยสร้างตัวละครในเกมร่วมกับซานริโอ ที่บริษัทผลิตคอนเทนต์ Imagineer ในระยะแรก คัฟเวอร์มีจุดมุ่งหมายในด้านความเป็นจริงเสริม (AR) และความเป็นจริงเสมือน (VR) และได้รับทุนเริ่มต้นจาก Tokyo VR Startups และ Recruit

            ในช่วงท้ายของปี 2017 บริษัทได้แสดงโปรแกรมตัวอย่างที่สามารถตรวจจับการเคลื่อนไหวได้ สามารถถ่ายทอดสดได้ โดยทานิโงะได้กล่าวไว้ว่า ไอเดียสำหรับ 'ไอดอลเสมือนจริง' ที่ได้มานั้นมาจากตัวละครเสมือนจริงเช่น ฮัตสึเนะ มิกุ และ คิสึนะ ไอ ที่เป็นผู้ริเริ่ในการใช้ตัวละครเสมือนจริงบนยูทูปในปี 2016
            
            คัฟเวอร์ได้เดบิวต์ ときのそら (โทคิโนะ โซระ) ซึ่งเป็นวีทูปเบอร์คนแรกของบริษัทโดยใช้โปรแกรมตรวจจับการเคลื่อนไหวของบริษัทในวันที่ 7 กันยายน 2017 ในวันที่ 21 ธันวาคมของปีเดียวกัน บริษัทได้ปล่อยแอพลิเคชั่น โฮโลไลฟ์ ที่ทำให้ผู้ใช้สามารถดูการถ่ายทอดสดได้ทางเทคโนโลยี AR ในวันถัดมาคัฟเวอร์ได้เปิดการรับสมัครสำหรับวีทูปเบอร์คนที่ 2 ของบริษัทที่ได้รับโดยชื่ออย่างเป็นทางการว่า ロボ子 (โรโบโกะ) โดยได้รับการเดบิวต์ในวันที่ 4 มีนาคม 2018
        </p>
    </section>

    <section id="products">
        <h2>สินค้าของเรา</h2>
        <hr>
        <p>Shishiro Botan</p>
       
        <img src="https://shop.hololivepro.com/cdn/shop/files/hololivefriends_top_ShishiroBotan_9ff0abe7-a209-48f7-8dab-2b9fca958de1_large.png?v=1712154633" alt="Shishiro Botan" width="200">
        <img src="https://shop.hololivepro.com/cdn/shop/files/hololivefriends_vol.13_top_ShishiroBotanMidnightConvenienceStoreOutfit_1024x1024.png?v=1721267141" alt="Shishiro Botan Midnight" width="200">
        
    <figure>
        <hr>
        
        <img src="https://shop.hololivepro.com/cdn/shop/files/hololivefriends_vol.13_top_ShishiroBotanMidnightConvenienceStoreOutfit_1024x1024.png?v=1721267141" width="200"alt="สินค้าชิ้นที่ 2">
        
    <figcaption>
    โฮโลไลฟ์ เฟรนด์ส กับคุณ ชิชิระ โบตัน ชุดคอสตูมร้านสะดวกซื้อยามดึก
        </figcaption>
        </figure>
    </section>
    <hr>
    <a href="https://shop.hololivepro.com/cdn/shop/files/hololivefriends_vol.13_shohin_ShishiroBotanMidnightConvenienceStoreOutfit_large.png?v=1721267141">
        <img src="https://shop.hololivepro.com/cdn/shop/files/hololivefriends_vol.13_shohin_ShishiroBotanMidnightConvenienceStoreOutfit_large.png?v=1721267141images/products/product1.jpg" 
             alt="คลิกเพื่อดูรูปขนาดใหญ่"
             width="200">
    </a>
<hr>

    <a href="#top">กลับด้านบน</a>
    <a href="#products">ไปยังสินค้า</a>

    <a href="mailto:contact@example.com">ส่งอีเมลหาเรา</a>
    <a href="tel:+66812345678">โทร 081-234-5678</a>

    <a href="files/document.pdf" download>ดาวน์โหลดเอกสาร</a>

</body>
</html>
```
- ภาพผลลัพธ์:
[วางภาพ screenshot ที่นี่]
![lab 4-1](https://github.com/user-attachments/assets/f982070b-f70f-4719-8721-e2676b97570f)
![lab 4-2](https://github.com/user-attachments/assets/57ce4a3f-b30d-4472-bceb-100f58b75121)



