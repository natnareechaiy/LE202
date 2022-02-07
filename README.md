# **LE202 Micro1**
## **สรุป WEEK1**
### **Microcontroller**
  #### **Digital**
    การนำข้อมูลดิจิตอลมาใช้งาน คือการเอาสัญญาณไฟฟ้ามาแทนด้วยตัวเลข โดยตัวเลขเหล่านี้เรียกว่า 'ตัวเลขดิจิตอล' หรือ 'Binary' เป็นตัวเลขฐาน 2 ซึ่งมีแค่ 0 และ 1
    ดังนั้นการนำมาใช้ทางไฟฟ้าคือทำให้รู้ว่าสัญญาณ on หรือ off, มีแรงดันหรือไม่มีแรงดัน นอกจากนี้ยังสามารถนำสัญญาณดิจิตอลมาใช้ในตัวอักษรได้อีกด้วย
  #### **Voltage**
    แรงดันไฟฟ้า คือ ความต่างศักย์ไฟฟ้าระหว่างจุด 2 จุด มีหน่วยเป็นโวลต์(V)
  #### **Computer**
    คอมพิวเตอร์มีหลายแบบ ทั้งคอมพิวเตอร์ขนาดใหญ่ ขนาดกลางซึ่งใช้กันตามบ้าน ขนาดเล็ก(Single board computer) 
    และขนาดจิ๋ว(Microcontroller)ซึ่งใช้ในการเชื่องโยงIoT
  #### **Internet**
    Internet สามารถทำให้ทุกอย่างเชื่อมโยงกันได้ทั้งไร้สายและมีสาย เช่น wifi 4g 5g
  #### **Program language**
    การพัฒนาซอฟแวร์ให้ามารถทำงานบนคอมพิวเตอร์เมื่อ 50-70 ปีที่แล้ว เริ่มต้นจากภาษา assembly และภาษาC ปัจจุบันมีภาษาสำหรับพัฒนาโปรแกรมอีกมากมาย
  #### **PlatformIO**
    PlatformIO คือ Platform สำหรับเขียนโปรแกรมบน microcontroller ที่รวบรวมที่รวบรวมเอา IDE (Integrated Develpment Environment) 
    และ Boards ต่างๆมาไว้ที่เดียวกัน เหมาะสำหรับผู้ที่พัฒนาด้าน IoT ในอนาคต นอกจากนี้ใน PlatformIO ยังมีโปรแกรมที่สามารถนำมาประยุกต์ใช้ได้ทันที
    ไม่ต้องเขียนโปรแกรมใหม่อีกกว่า 10,000 รายการ
  #### **iotset1**
    การเตรียมเพื่อพัฒนา microcontroller
    เปิด browser เข้าลิงก์ https://github.com/choompol-boonmee/iotset1
    เพื่อ download โปรแกรม git หลังจากนั้นให้ทำตามคำสั่งในลิงก์
### **Experiment**
  #### **Run Example 1**
    ในการเขียนโปรแกรมลง microcontroller ESP-01 ซึ่งมีเสาอากาศสำหรับ wifi ต้องทำการเสียบกับ Serial port หลังจากนั้นให้ดูตัวอย่างโปรแกรม
    จากโฟลเดอร์ pattani ซึ่งจะมีโปรแกรมตัวอย่าง 9 โปรแกรม ในตัวอย่างแรกจะใช้โปรแกรม 01_Serial-Monitor สำหรับโปรแกรมจะมี 15 บรรทัด 
    2 ฟังก์ชัน คือ setup ซึ่งจะ run ครั้งเดียว และส่วนของ loop ซึ่งจะ run วนลูปตลอดไป
    ในส่วนของ setup จะ set serial port ที่ความเร็ว 115200 และในส่วนของ loop จะให้เพิ่มตัวแปร count (cnt) ขึ้นเรื่อยๆ โดยให้แสดงผลตัวแปร cnt ออกมา 
    และให้หน่วงเวลา 1 วินาที หรือ 1000 ms
    โดยวิธีการ upload โปรแกรมลง microcontroller จะใช้คำสั่ง pio run -t upload เมื่อโปรแกรมพร้อมทำงานจะใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์
    สำหรับการ reset ให้กดปุ่มสีแดง
  #### **Run Example 2**
    ในโปรแกรมที่ 2 นี้มี 2 ส่วน คือส่วนของ setup เพื่อเตรียม set wifi ให้พร้อมทำงาน และส่วนของ loop เพื่อวนลูปตลอดไป โดยมีการแสดงผลว่า
    "เริ่มต้นแสกนหา wifi"
    ในการ upload โปรแกรม จะใช้คำสั่ง pio run -t upload  เพื่อให้โปรแกรม upload ต้องกดปุ่มสีดำหรือ port 0 แล้วกดปุ่ม reset สีแดง
    เมื่อ upload เสร็จ จะใช้คำสั่ง pio device monitor เพื่อดูว่าพบ wifi อะไรบ้าง
 #### **Run Example 3**
    โปรแกรมที่ 3 เป็นโปรแกรมสำหรับทดลองการ output สัญญาณออกไปภายนอก ซึ่งมี output port และ input port คือ 0 และ 1
    หากต้องการเขียนโปรแกรมลง microcontroller ต้องนำมาเสียบกับ USB 2.0 serial port โดยต้องเสียบผ่าน adaptor โดยสีขาวจะเป็น port 0
    และสีเหลืองจะเป็น port 1 เพื่อให้ port 0 ซึ่่งเป็น output สามารถมองเห็นได้ด้วยตา จึงนำมาต่อกับ LED เพื่อให้มีแสงสว่างเมื่อมีการส่งสัญญาณ 1 มาที่ port 
    
    จากเนื้อหาของโปรแกรม โปรแกรมจะ set ให้ port 0 เป็น output หลังจากนั้นใช้คำสั่ง loop เพื่อให้วนลูปทุกครึ่งวินาที หรือ 500 ms แล้วนับ count(cnt) ไปเรื่อยๆ
    ถ้า cnt เป็นเลขคี่จะหมายถึง ON แต่ถ้าเป็นเลขคู๋จะหมายถึง OFF หลังจากนั้นใช้คำสั่ง upload โปรแกรม และเพื่อให้โปรแกรมถูก upload 
    ต้องกดปุ่มสีดำ หลังจากนั้นกดปุ่ม reset สีแดง ถ้าต้องการดูผลการ run ใช้คำสั่ง pio device monitor จะพบว่าทุกครึ่งวินาทีจะสลับ ON-OFF ไปเรื่อยๆ 
    และไฟ LED ที่ port 0 จะเปล่งแสงในช่วง ON
   
   **Run relay**
    
    นำ microcontroller ที่ถูกลงโปรแกรมไว้แล้วมาเสียบกับ relay เพื่อให้ส่งสัญญาณไปควบคุม relay ให้เปิด-ปิดสวิตช์ หลังจากนั้นนำ relay ที่เสียบกับ 
    microcontroller ไปต่อกับขั้วชาร์จ หรือ power bank เพื่อจ่ายไฟให้ สัญญาณไฟก็จะควบคุม relay ให้ทำงานเปิด-ปิดทันที
    และจะได้ยินเสียงหน้าสัมผัสสวิตช์ซึ่งเป็นโลหะ เอาไว้เป็นตัวนำไฟฟ้า
    
 #### **Run Example 4**
    โปรแกรมที่ 4 เป็นการทดลองนำสัญญาณ input จากภายนอกเข้ามาใน microcontroller โดยตัวโปรแกรมจะแบ่งเป็น 2 ส่วน คือ
    ส่วนของ setup จะ set ให้ port 0 สีขาวเป็น input และ port 2 สีเหลืองเป็น output ในส่วนของ loop โปรแกรมก็จะวนลูปไปเรื่อยๆ จากนั้นนำโปรแกรม
    ไป upload ลง microcontroller เมื่อ upload เสร็จ โปรแกรมจะเช็คที่ port 0 ถ้า output เป็น 0 หลอดไฟจะสว่าง แต่ถ้าเป็น 1 หลอดไฟจะดับ หลังจากนั้นเราจะนำ
    microcontrollerที่ถูกลงโปรแกรม มาต่อกับ Sensorที่ถูกต่ออยู่กับตัวต้านทาน โดนนำตัวsensorมาต่อที่ไฟเลี้ยง 3V ส่วนอีกขาต่อกับเส้นสีดำ หรือ ground
    ผลลัพธ์ที่ได้คือ ถ้า sensor ได้รับแสงสว่าง ค่าที่แสดงออกมาจะเป็น 0 และไฟจะติด แต่ถ้า sensor โดนบังแสงค่าที่แสดงออกมาจะเป็น 1 และไฟจะดับ
 #### **Run WiFi**
    เป็นโปรแกรมที่สร้าง web server ผ่าน wifi เนื่องจากต้องเชื่อมต่อกับ wifi จึงต้องใส่ชื่อ wifi และ password ลงในโปรแกรม โดยตัวโปรแกรมจะมี 2ส่วน คือ
    ส่วน setup และ ส่วนของ loop ซึ่งในการทดสอบโปรแกรมนี้จะต้องมีการใช้ web browser ด้วย
 #### **Run WiFi Access Point**
    สำหรับโปรแกรมนี้มีความแตกต่างกับ โปรแกรมที่ 5 คือในโปรแกรมนี้ไม่จำเป็นต้องเชื่อมต่อกับ wifi ที่มีอยู่แล้ว แต่สามารถสร้าง wifi access point ขึ้นมาเองได้
    ในการทดลองโปแกรมนี้เราใช้ microcontroller ESP-01 ซึ่งมี wifi ในตัวเองเป็น access point เราต้องกำหนดชื่อให้ wifi ของเราด้วย 
    สำหรับตัวโปรแกรม จะมีการสร้าง access point โดยการ run คำสั่ง softAP(ssid,password) โดยกำหนดชื่อ และ password เอง หลังจากนั้น run โปรแกรมโดยการ
    upload ลง microcontroller เมื่อโปรแกรม run ได้ จะสร้าง access point ขึ้นมา โดยไม่ต้องใช้ access point ที่อื่น
    สำหรับการทดสอบ อาจใช้คอมพิวเตอร์หรือโทรศัพท์มือถือในการเช็คว่า wifi นั้นมีจริงหรือไม่
