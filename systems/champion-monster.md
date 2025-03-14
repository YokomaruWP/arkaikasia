---
description: >-
  มอนสเตอร์แชมป์คือมอนสเตอร์ที่ถูกเรียกขึ้นมาโดยเซิร์ฟเวอร์เมื่อมีเงื่อนไขบางอย่างถูกต้อง
---

# 🏆 มอนสเตอร์แชมป์

<figure><img src="../.gitbook/assets/mmmm.gif" alt=""><figcaption><p><mark style="color:red;"><strong>มอนสเตอร์แชมป์ในแอ็คชั่น</strong></mark></p></figcaption></figure>

## **ลักษณะเฉพาะ**

* เมื่อมี **แชมป์** ปรากฏขึ้น จะมีการประกาศให้ผู้เล่นทั้งหมดในแผนที่ทราบ
* **แชมป์ให้ประสบการณ์มากขึ้น 30 เท่าและมีอัตราการดรอปไอเทมมากขึ้น 10 เท่า**

***

## **สูตรการเรียก**

การคำนวณที่ใช้เมื่อฆ่ามอนสเตอร์เพื่อกำหนดว่ามอนสเตอร์จะถูกเรียกเป็นแชมป์หรือไม่นั้นมีดังนี้:

```
mathematicaCopiarEditarSummon Chance += [(Monster Level / 100) * Number of Players on the Map]%
```

### **ตัวอย่าง:**

\
ถ้าคุณอยู่ในกลุ่มกับเพื่อน 5 คนในแผนที่และฆ่ามอนสเตอร์ระดับ 25 **25 ครั้ง** ดังนั้น:

โอกาสที่มอนสเตอร์นี้จะกลายเป็นแชมป์คือ **1.25%**.

ถ้าการเรียกไม่เกิดขึ้น โอกาสถัดไปจะเพิ่มขึ้นเป็น **2.50%** และต่อไปเรื่อยๆ

***

## **ประเภทของแชมป์**

* ประเภทของแชมป์ที่ถูกเรียกขึ้นมานั้นเป็นแบบสุ่ม ตารางด้านล่างแสดงลักษณะของมอนสเตอร์แต่ละตัว

<table><thead><tr><th width="102">ประเภท</th><th width="92">ความเสียหาย</th><th width="151">สุขภาพ</th><th width="147">การต้านทาน</th><th>ฟีเจอร์</th></tr></thead><tbody><tr><td><mark style="background-color:green;">Ventus</mark></td><td>+7%</td><td>30</td><td>ลม = 90%</td><td>ไม่มี</td></tr><tr><td><mark style="background-color:yellow;">Solid</mark></td><td>+7%</td><td>700</td><td>ดิน = 90%</td><td>1% โอกาสในการทำลายอาวุธ</td></tr><tr><td><mark style="background-color:purple;">Necro</mark></td><td>+7%</td><td>1500</td><td>ซากศพ = 90%</td><td>ฟื้นฟู 3% ของ HP ของม็อบ</td></tr><tr><td><mark style="background-color:orange;">Fairer</mark></td><td>+7%</td><td>ไม่สามารถถูกขัดจังหวะ</td><td>ไฟ = 90%</td><td>มี [Endure] ทำงานอยู่</td></tr><tr><td><mark style="background-color:blue;">Elusive</mark></td><td>+7%</td><td>ไม่สามารถถูกขัดจังหวะ</td><td>ไม่มี</td><td>ไม่รับความเสียหายทางกายภาพ</td></tr></tbody></table>

## **ข้อกำหนดของระบบ**

<table><thead><tr><th width="169">ข้อกำหนด</th><th>ประเภท</th></tr></thead><tbody><tr><td>ลิงก์</td><td>ไม่มี</td></tr><tr><td>ข้อจำกัด</td><td>ไม่ทำงานกับ <strong>มอนสเตอร์ระดับตำนาน</strong> และมีเพียง <strong>มอนสเตอร์แชมป์</strong> หนึ่งตัวที่ถูกเรียกขึ้นมาในขณะที่อีกตัวยังมีชีวิตอยู่ในแผนที่เดียวกัน</td></tr></tbody></table>