---
name: requirement-to-backlog
description: Analyze the requirement documents under docs/01-requirements/01-spec/ and produce a prioritized Product Backlog (Epics, User Stories, Acceptance Criteria) under docs/01-requirements/02-plan/. Use when asked to "สร้าง Product Backlog", "แตก Requirement เป็น Backlog", or to update the backlog after the requirement doc changes.
---

# Requirement to Backlog

แปลงเอกสาร Requirement ให้เป็น Product Backlog ที่จัดลำดับความสำคัญแล้ว ตามแนวทาง Agile/Scrum ของโปรเจกต์นี้

## ขั้นตอน

1. อ่านเอกสารทั้งหมดใน `docs/01-requirements/01-spec/` เพื่อทำความเข้าใจ scope, Epic, และเงื่อนไขทางธุรกิจ
2. ถ้า spec ยังไม่มีเนื้อหาจริง หรือขาดรายละเอียดที่จำเป็นต่อการแตก backlog (เช่น ไม่รู้กลุ่มผู้ใช้ หรือฟีเจอร์หลัก) ให้ถามผู้ใช้ก่อน อย่าสร้าง requirement ขึ้นมาเอง
3. แตกแต่ละ Epic ในสเปคให้เป็น User Story รูปแบบ:
   `ในฐานะ [บทบาทผู้ใช้], ฉันต้องการ [สิ่งที่ต้องการ], เพื่อที่จะ [เหตุผล/คุณค่า]`
4. เขียน Acceptance Criteria ของแต่ละ User Story เป็น checklist สั้นๆ ที่ตรวจสอบได้จริงว่า "เสร็จ" เมื่อไหร่
5. จัดลำดับความสำคัญ (Priority: สูง/กลาง/ต่ำ) ตามคุณค่าที่ส่งมอบให้ผู้ใช้/ธุรกิจ ไม่ใช่ตามความง่ายในการพัฒนา
6. เขียนผลลัพธ์ลงไฟล์ `docs/01-requirements/02-plan/product-backlog.md` เป็นตารางคอลัมน์: ID, Epic, User Story, Priority, Acceptance Criteria, Status (ยังไม่เริ่ม/กำลังทำ/เสร็จแล้ว)
7. อัปเดต `docs/01-requirements/02-plan/index.md` และ `docs/01-requirements/01-spec/index.md` ให้ลิงก์ (wikilink) ไปยังไฟล์ที่สร้าง/แก้ไข ถ้ายังไม่มีลิงก์

## กฎ

- ใช้ภาษาไทย ให้ตรงกับเอกสารอื่นในโปรเจกต์
- ห้ามลบ backlog item เดิมที่มีอยู่แล้วโดยไม่ถามก่อน ถ้า item ไหนไม่ relevant แล้วให้ย้ายไป `docs/00-archived/` แทนการลบ
- Backlog เป็นของที่เปลี่ยนแปลงได้เรื่อยๆ (living document) ไม่ต้องทำให้สมบูรณ์แบบในครั้งเดียว
