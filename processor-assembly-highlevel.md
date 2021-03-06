# ภาษาขั้นสูง (high level language)
   เป็นภาษาที่ถูกสร้างขึ้นมาเพื่อให้สามารถเขียน และอ่านโปรแกรมได้ง่ายขึ้น เนื่องจากมีลักษณะเหมือนภาษาอังกฤษทั่วๆไป และผู้เขียนโปรแกรม ไม่จำเป็นต้องมีความรู้เกี่ยวกับ ระบบฮาร์ดแวร์แต่อย่างใด
#### ตัวอย่าง
     - ภาษาฟอร์แทรน(Fortran)
     - โคบอล (Cobol)
     - ภาษาเบสิก (BASIC) 
     - ภาษาวิชวลเบสิก (Visual Basic)
     - ภาษาซี (C)
     - ภาษาจาวา (Java)
     
 # Processor, Microcontroller
 ## Processor
   หน่วยประมวลผลกลาง (Central Processing Unit) หรือ CPU (ซีพียู) หรือ โปรเซสเซอร์ (Processor) เป็นองค์ประกอบที่สำคัญส่วนหนึ่งของเครื่องคอมพิวเตอร์ทุกประเภท เปรียบเสมือนกับเป็นมันสมองให้กับคอมพิวเตอร์นั่นเอง ประกอบไปด้วยวงจรทางไฟฟ้ามากมายที่อยู่บนแผ่นซิลิกอนซิปซึ่งมีขนาดเล็กมาก ๆ
 ### หลักการทำงาน
     ในการทำงานของ cpu หรือโปรเซสเซอร์นั้น เมื่อมีการรับข้อมูลเข้ามาจะนำไปเก็บไว้ในหน่วยความจำก่อนแล้วอ่านค่าจากหน่วยความจำ
     จากนั้นcpuก็จะประมวลผลอีกทีว่ามีคำสั่งจะให้ทำอะไร ที่ไหน เช่น ถ้าข้อมูลที่ได้รับมาเป็นการคำนวณทางคณิตศาสตร์ก็จะถูกส่งให้ไปที่หน่วย EXECUTION UNIT 
     เมื่อกระทำคำสั่งในขั้นตอนนี้แล้ว มีการคำนวณทางด้านคณิตศาสตร์เกิดขึ้นแบบง่าย ๆ ก็จะทำการคำนวณให้เสร็จสิ้น แล้วส่งออกสู่การแสดงผล
 ## Microcontroller
   ไมโครคอนโทรลเลอร์ คือ อุปกรณ์ควบคุมขนาดเล็ก ซึ่งบรรจุความสามารถที่คล้ายคลึงกับระบบคอมพิวเตอร์ โดยในไมโครคอนโทรลเลอร์ได้รวมเอาซีพียู, หน่วยความจำ และพอร์ต ซึ่งเป็นส่วนประกอบหลักสำคัญของระบบคอมพิวเตอร์เข้าไว้ด้วยกัน โดยทำการบรรจุเข้าไว้ในตัวเดียวกัน
 ### หลักการทำงาน
    หลักการทำงานหลักๆของไมโครคอนโทรลเลอร์คือจะนำมาใช้ในการควบคุมระบบหรืออุปกรณ์ต่างๆ และสามารถนำมาประยุกต์ใช้งานได้อย่างหลากหลาย
    โดยผ่านการออกแบบวงจรให้เหมาะกับลักษณะงานนั้นๆ และสามารถรับโปรแกรมคำสั่งภาษาซี เพื่อควบคุม INPUT/OUTPUT 
    ในการสั่งงานไปควบคุมระบบหรืออุปกรณ์นั้นๆ สามารถใช้ได้ทั้งระบบAnalog และ ระบบDigital
    
 # ภาษาAssembly (low level language)
 หมายถึง ภาษาที่ใช้ในการเขียนโปรแกรมภาษาหนึ่งซึ่งจะตรงเข้าไปจัดการกับตัวไมโครโพรเซสเซอร์ หรือ "ตัวประมวลผล" ของเครื่องคอมพิวเตอร์ และจะทำการประมวลผลโดยตรงได้เลย โดยปกติ ภาษานี้จะเรียนยากและต้องเขียนยาวกว่าภาษา C หรือภาษา BASIC แต่จะทำให้ได้ผลลัพธ์ (result) เร็วกว่า และใช้เนื้อที่เก็บน้อยกว่าโปรแกรมภาษาอื่นมาก นิยมใช้ภาษานี้เมื่อต้องการประหยัดเวลาทำงานของเครื่องคอมพิวเตอร์ และเพิ่มประสิทธิภาพของโปรแกรม โดยไม่ต้องพะวงถึงความชัดเจนมากนัก และที่สำคัญก็คือ โปรแกรมภาษานี้จะเขียนขึ้นมาเพื่อใช้เฉพาะกับเครื่องใดเครื่องหนึ่ง หากจะนำไปใช้กับเครื่องคนละรุ่น ก็จะต้องมีการปรับแก้ก่อน (ขึ้นกับหน่วยประมวลผลหรือ CPU)
 
 # ภาษาเครื่อง (Machine language)
 ภาษาเครื่อง เป็นภาษาโปรแกรมคอมพิวเตอร์ระดับต่ำที่สุด ซึ่งคอมพิวเตอร์เข้าใจได้ทันทีโดยไม่ต้องผ่านตัวแปลภาษาเพราะเขียนคำสั่งและแทนข้อมูลด้วยเลขฐานสอง (Binary Code) ทั้งหมด ซึ่งเป็นการเขียนคำสั่งด้วยเลข 0 หรือ 1
 #### ข้อดี
    1. สามารถเขียนโปรแกรมควบคุมการทำงานคอมพิวเตอร์ได้โดยตรง
    2. สั่งงานให้คอมพิวเตอร์ทำงานได้อย่างรวดเร็ว
 #### ข้อเสีย
    1. ต้องเขียนโปรแกรมคำสั่งยาวทำให้ผิดพลาดได้ง่าย
    2. ผู้เขียนโปรแกรมจะต้องรู้ระบบการทำงานของเครื่องเป็นอย่างดีจึงสามารถเขียนโปรแกรมได้ และถ้าเครื่องที่มีฮาร์ดแวร์ต่างกัน จะใช้โปรแกรมร่วมกันได้
    
# ความสัมพันธ์
        เริ่มแรกนั้นการสั่งให้คอมพิวเตอร์ทำงาน ต้องเขียนคำสั่งอยู่ในรูปของเลขฐานสอง ซึ่งประกอบด้วยเลข 0 และ 1 
    จึงทำให้การเขียนโปรแกรมควบคุมการทำงานของคอมพิวเตอร์ยุ่งยากมาก เพราะถ้าเข้ารหัสผิดพลาด การทำงานของคอมพิวเตอร์ก็จะผิดพลาด 
    หรือได้ผลลัพธ์ไม่ตรงตามจุดประสงค์ที่ต้องการ มนุษย์จึงพัฒนารูปแบบของภาษาขึ้นมาใหม่โดยใช้รหัสข้อความในภาษาอังกฤษที่เข้าใจได้ง่ายนั่นคือภาษา Assembly
    แต่เนื่องจากเป็นภาษาที่เขียนยาก จึงมีการพัฒนาภาษาขั้นสูงขึ้นมา ซึ่งสามารถเรียกได้ว่าเป็นภาษารุ่นที่ 3 
    
        ไมโครคอนโทรลเลอร์นั้นถือได้ว่าเป็นคอมพิวเตอร์ขนาดเล็กที่มีโปรเซสเซอร์และส่วนประกอบอื่น ๆ เพื่อให้เป็นคอมพิวเตอร์ อย่างไรก็ตามจะพบว่าภาษา C ซึ่งเป็นภาษาขั้นสูง
    เป็นภาษาที่นักพัฒนางานทางด้านไมโครคอนโทรลเลอร์นำมาประยุกต์ใช้งานอย่างแพร่หลาย จะเห็นได้ว่าบริษัทที่ผลิตไมโครคอนโทรลเลอร์ส่วนใหญ่เลือกใช้ภาษาซี
    ในการพัฒนาโปรแกรมและมีนักพัฒนาได้เขียนโค้ดต้นฉบับภาษาซีรองรับการประยุกต์ใช้งานไว้เป็นจำนวนมาก
