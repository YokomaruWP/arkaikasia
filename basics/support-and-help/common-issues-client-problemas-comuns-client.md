---
description: >-
  หากคุณไม่พบวิธีแก้ปัญหาด้านล่างนี้ กรุณาติดต่อทีมสนับสนุนของเราทาง
  Discord หรือ WhatsApp
---

# 🪛 ปัญหาทั่วไป (Client)

## Arkaik.exe เปิดขึ้น แต่เมื่อคลิก "Play" ไม่มีอะไรเกิดขึ้น และมันปิดตัวลง

**สาเหตุ:**

* โปรแกรม **แอนตี้ไวรัส** หรือ **การป้องกันการโจมตี** ของคุณอาจบล็อกไฟล์ `.exe` ของไคลเอนต์

**วิธีแก้ไข:**\
ไปที่:\
➡ **Windows Security** > **App & Browser Control** > **Exploit Protection Settings** > **Program Settings (แท็บด้านบน)** > **(+) เพิ่มโปรแกรมเพื่อปรับแต่ง**

พิมพ์ `Client.exe` และเปิดใช้งานกระบวนการทั้งหมด (ตรวจสอบกล่องเลือกทั้งหมด; บางกล่องอาจเปิดใช้งานโดยค่าเริ่มต้น—ปิดใช้งานด้วยถ้าจำเป็น)\
<figure><img src="../../.gitbook/assets/image (149).png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (150).png" alt="" width="410"><figcaption></figcaption></figure>

## **Arkaik.exe ไม่เปิด ไม่อยู่ในตัวจัดการงาน และไม่มีข้อผิดพลาดปรากฏ**

**สาเหตุ:**

* โปรแกรม **แอนตี้ไวรัส** หรือ **การป้องกันการโจมตี** ของคุณอาจบล็อกไฟล์ `exe` ของ **Arkaik**

**วิธีแก้ไข:**\
➡ **Windows Security** > **App & Browser Control** > **Exploit Protection Settings** > **Program Settings (แท็บด้านบน)** > **(+) เพิ่มโปรแกรมเพื่อปรับแต่ง**

พิมพ์ **Arkaik.exe** และเปิดใช้งานกระบวนการทั้งหมด (ตรวจสอบกล่องเลือกทั้งหมด; บางกล่องอาจเปิดใช้งานโดยค่าเริ่มต้น—ปิดใช้งานด้วยถ้าจำเป็น)

📌 **ภาพ:** ขั้นตอนเดียวกันกับข้างต้น!

## **ข้อผิดพลาด: ไม่สามารถค้นหาไฟล์ที่มีอักขระพิเศษ "????"**

**ปัญหา:**

* เมื่อเรียกใช้ `Client.exe` หลังจากเลือกตัวละคร เกมจะแสดงอักขระพิเศษเป็น `???` ทำให้เกม **แครช**

<figure><img src="../../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

**สาเหตุ:**

* แพ็คเกจภาษาล้มเหลวในการแปลงการเข้ารหัส UTF-8 สำหรับอักขระ **เกาหลี (Western Europe 1252)**

**วิธีแก้ไข:**\
➡ **Control Panel** > **เปลี่ยนวันที่ เวลา หรือรูปแบบตัวเลข** > **Administrative (แท็บด้านบน)** > **เปลี่ยนระบบภูมิภาค**

🔹 **ยกเลิกการเลือก** กล่อง **UNICODE UTF-8** หากเปิดใช้งานอยู่ รีสตาร์ท และทดสอบเกม

<figure><img src="../../.gitbook/assets/image (152).png" alt="" width="329"><figcaption></figcaption></figure>

## **ข้อผิดพลาดใน Client.exe: "Cannot init d3d OR grf file has problem" หรือหน้าจอขาว**

<figure><img src="../../.gitbook/assets/Cannot_init_d3d_or_grf_file_has_problem.png" alt="" width="188"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/800px-Telabranca.png" alt="" width="375"><figcaption><p>หน้าจอขาว</p></figcaption></figure>

**ปัญหา:**

* เมื่อคลิกที่ **Client.exe** ไม่มีอะไรเกิดขึ้น หน้าจอขาวปรากฏขึ้น และเกมปิดทันที แม้หลังจากเลือก **การ์ดกราฟิก** ใน **RO/OpenSetup.exe**

**ปัญหา 2:**

* เมื่อคลิก **Play** ผ่าน **Arkaik.exe** หรือ **Client.exe** ข้อความแสดงข้อผิดพลาด **"Cannot init d3d OR grf file has problem"** ปรากฏขึ้น (นี่คือกรณีที่พบบ่อยที่สุด)

***

#### **วิธีแก้ไขสำหรับปัญหา 2:**

1. เปิด **RO/OpenSetup.exe**
2. เลือก **การ์ดกราฟิก** ของคุณ
3. คลิก **Apply**

➡ หากปัญหายังคงอยู่ ลองใช้ **วิธีแก้ไข 1** ด้านล่าง

#### **สาเหตุที่เป็นไปได้:**

* ไดรเวอร์ **การ์ดกราฟิก** ของคุณอาจล้าสมัยหรือไม่ถูกตรวจพบโดย **Ragnarok**
* แล็ปท็อปบางรุ่น **RTX 3050** จาก **Asus Gaming** มีปัญหานี้

***

#### **วิธีทดสอบปัญหานี้:**

1. **คลิกขวา** ที่ **Client.exe**
2. เลือก **"Troubleshoot Compatibility"**
3. คลิก **"Test the Program"**

หากเกม **ทำงานแต่มีข้อผิดพลาด** (_เช่น ขาดพื้นผิวหรือภาพไม่ถูกต้อง_) ให้ดำเนินการไปยัง **วิธีแก้ไขถัดไป**

<figure><img src="../../.gitbook/assets/image (153).png" alt="" width="387"><figcaption></figcaption></figure>

\
**วิธีแก้ไขเพิ่มเติม: "Cannot init d3d OR grf file has problem"**

**วิธีแก้ไข:**

1. เปิด **Device Manager**
2. ไปที่ **Display Adapters**
3. **ปิดการใช้งาน** **การ์ดกราฟิก RTX** ของคุณ (หรือ GPU ที่แยกต่างหาก)
4. เปิด **Client.exe** อีกครั้ง

**คำอธิบาย:**

* หากเกม **เปิดและทำงาน** แสดงว่ากำลังใช้ **Vodoo** renderer
* การ์ดกราฟิกของคุณอาจ **ทันสมัยเกินไป** และ **ไม่รองรับ DirectX เวอร์ชันเก่า**

[<mark style="color:purple;">Link do Video Tutorial</mark>](https://www.youtube.com/watch?v=2dStctdLMeE)

<figure><img src="../../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

## **ข้อผิดพลาดในการโหลดโมดูล Arkaik.exe ก่อนหน้าจอเข้าสู่ระบบ (วันที่ & เวลา)**

**ปัญหา:**

* เมื่อเปิด **Arkaik.exe** ในระหว่างกระบวนการโหลดโมดูล จะมีข้อผิดพลาด **สีแดง** ปรากฏขึ้นว่า:\
  &#xNAN;**"Server failed to authenticate the request"**.

<figure><img src="../../.gitbook/assets/image (155).png" alt="" width="563"><figcaption></figcaption></figure>

**สาเหตุ:**

* ปัญหานี้พบได้บ่อยใน **Windows 11** เนื่องจากต้องพึ่งพาเซิร์ฟเวอร์ออนไลน์เพื่อซิงโครไนซ์เวลาของระบบ

**วิธีแก้ไข:**

1. **ไปที่:**
   * **Control Panel** > **วันที่ & เวลา** > **ซิงค์ตอนนี้**

<figure><img src="../../.gitbook/assets/image (156).png" alt="" width="332"><figcaption></figcaption></figure>

1. เปิดการตั้งค่า **วันที่ & เวลา** แบบคลาสสิกใน Windows
2. **ปรับวันที่และเวลา** ด้วยตนเอง
3. ตรวจสอบให้แน่ใจว่าเวลาตรงกับนาทีปัจจุบันจาก **บราซิล (Google Time Server)**
4. นอกจากนี้ให้เปิดใช้งาน:
   * **"เปลี่ยนเขตเวลา"**
   * **"เวลาอินเทอร์เน็ต"** ซิงโครไนซ์กับเซิร์ฟเวอร์ที่ถูกต้อง

**หากปัญหายังคงอยู่:**

<figure><img src="../../.gitbook/assets/image (157).png" alt=""><figcaption><p><mark style="color:red;"><strong>คลิกที่เวลาอินเทอร์เน็ต</strong></mark></p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (158).png" alt=""><figcaption><p><mark style="color:red;"><strong>เปลี่ยนเขตเวลา</strong></mark></p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

## **ข้อผิดพลาด: ไม่สามารถรับ URL อัปเดต (เมื่อเปิด arkaik.exe)**

**ปัญหา:** เมื่อเรียกใช้ **arkaik.exe** จะมีข้อผิดพลาดในการอัปเดตปรากฏขึ้น: **"Failed to get updates URL"** ซึ่งหมายความว่าเซิร์ฟเวอร์อัปเดตปฏิเสธการเชื่อมต่อ

**วิธีแก้ไข:** ดาวน์โหลด **https://1.1.1.1** หากปัญหายังคงอยู่ **Cloudflare** สามารถปรับเส้นทางที่ดีที่สุดสำหรับอินเทอร์เน็ตของคุณได้

<figure><img src="../../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

## **หน้าจอสี่เหลี่ยมสีเมื่อเรียกใช้ Client.exe**

<figure><img src="../../.gitbook/assets/800px-Tela_com_quadrados_coloridos_arkaik_online.png" alt="" width="563"><figcaption></figcaption></figure>

**ปัญหา:**

* การตั้งค่านี้ถูกออกแบบมาสำหรับ **การ์ดกราฟิกเก่า** การ์ด **RTX** และ **ชิปเซ็ต** ใหม่อาจประสบปัญหานี้

**วิธีแก้ไข:**

1. ไปที่โฟลเดอร์ที่คุณติดตั้งเกม:
   * **ArkaikOnline/RO/OpenSetup.exe**
   * หรือเปิด **arkaik.exe** > **การตั้งค่า** > **External ROSETUP**
2. มองหากล่องเลือกที่มีชื่อว่า **"เปิดใช้งานเร่งความเร็วฮาร์ดแวร์"** **ปิดใช้งาน** บันทึก และรีสตาร์ทเกม
3. หากปัญหายังคงอยู่ ให้กลับไปที่ตำแหน่งเดียวกันและ:
   * **เพิ่มการ์ดกราฟิก**
   * **ตั้งค่าความละเอียดต่ำกว่า 1366x768**