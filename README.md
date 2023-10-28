# BEEP WITH ULTRASONIC SENSOR
&emsp;&emsp;โครงงานนี้จัดทำขึ้นเพื่อเป็นส่วนหนึ่งของวิชา Computer Programming เพื่อให้ได้ศึกษาหาความรู้ในเรื่องของการเขียนโปรแกรมภาษาC และการต่อบอร์ด Arduino โดยได้ศึกษาผ่านแหล่งความรู้ต่างๆ ไม่ว่าจะเป็นการศึกษาในห้องเรียนหรือการศึกษาด้วยตนเอง อาทิเช่น แหล่งความรู้จากเว็บไซต์ต่างๆ เป็นต้น ซึ่งในปัจจุบัน IoT (Internet of Things) ได้เข้ามามีบทบาทในชีวิตประจำวันเป็นอย่างมาก คณะผู้จัดทำจึงได้นำความรู้ทั้งหมดมาประยุกต์ใช้ทำโครงงานนี้ ซึ่งโครงงานที่จะนำเสนอนี้เป็นโครงงานทอยลูกเต๋าออนไลน์ เพื่อเพิ่มความสะดวกสบายในการใช้และช่วยลดทรัพยากรต่างๆ เนื่องจากลูกเต๋าเป็นสิ่งของที่มีขนาดเล็กทำให้เกิดการสูญหายและสิ้นเปลืองได้ง่าย ซึ่งผู้จัดทำคาดหวังเป็นอย่างยิ่งว่าการจัดทำโครงงานนี้จะมีข้อมูลที่เป็นประโยชน์ต่อผู้ที่สนใจศึกษาการพัฒนาเทคโนโลยีที่เกี่ยวข้องกับ IoT ต่อไปในอนาคต

# Poster
<img src="https://github.com/MyNNeiei/AboutC_project/blob/main/%E0%B9%82%E0%B8%9B%E0%B8%AA%E0%B9%80%E0%B8%95%E0%B8%AD%E0%B8%A3%E0%B9%8C.png" width="100%">

# ที่มาของโครงงาน
&emsp;&emsp;ในปัจจุบันอินเทอร์เน็ตได้เข้ามามีบทบาทในชีวิตประจำวันของเราเป็นอย่างมาก และคนส่วนใหญ่มีการใช้อินเทอร์เน็ตกันมากขึ้น ทางคณะผู้จัดทำจึงได้นำความรู้เกี่ยวกับการต่อบอร์ด
Arduino มาสร้างโครงงานการทอยลูกเต๋าออนไลน์ เนื่องจากลูกเต๋าเป็นสิ่งที่มีขนาดเล็กอาจทำให้เกิดการสูญหายได้หากต้องซื้อใหม่จะเป็นการสิ้นเปลืองเงินและทรัพยากร จึงได้ตัดสินใจจัดทำโครงงานนี้ขึ้นมาเพื่อเพิ่มความสะดวกสบายให้แก่ผู้ใช้งาน

# จุดประสงค์
- เพื่อให้ได้รับความสะดวกและรวดเร็วในการทอยลูกเต๋ามากยิ่งขึ้น
- เพื่อให้ได้ใช้เป็นสื่อในการเรียนการสอนในด้านต่างๆ
- สามารถสร้างวงจรจำลองการทอยลูกเต๋า

# ประโยชน์
- สามารถนำไปประยุกต์ใช้ตามชีวิตประจำวันได้จริง และสามารถนำไปประยุกต์ใช้งานให้เกิดประโยชน์ในอนาคตได้
- สามารถทอยลูกเต๋าได้โดยที่ไม่จำเป็นทอยลูกเต๋า เพื่อไม่ให้เกิดการเปลืองทรัพยากร
- ได้ฝึกการเขียนโปรแกรมด้วยภาษาC
- สามารถนำการต่อบอร์ด Arduino มาประยุกต์ใช้ได้

# อุปกรณ์
- Arduino UNO
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQsR8s4x-Aiywlqgw3OVy0u8jUW8uJ-V3mstw&usqp=CAU" width="150px">

- USB type A to USB type B
<img src="https://inwfile.com/s-fw/cr6shp.jpg" width="150px">

- BreadBoard
<img src="https://inwfile.com/s-fp/ottf4f.jpg" width="150px">

- สายจัมพ์เปอร์
<img src="https://www.tido.tech/wp-content/uploads/2020/09/%E0%B8%9C%E0%B8%B9%E0%B9%89-%E0%B9%80%E0%B8%A1%E0%B8%B5%E0%B8%A2.jpg" width="150px">

- Resistor 1k ohm
<img src="https://m.media-amazon.com/images/I/51l9hdTlmjL._SL1001_.jpg" width="150px">

- Resistor 220 ohm
<img src="https://commandronestore.com/products/products_img/BR200.png" width="150px">

- 7 Segment Display
<img src="http://www.warf.com/imagesitem/original/3517_1597.jpg" width="150px">

- Breadboard Small
<img src="https://cdn-shop.adafruit.com/970x728/65-00.jpg" width="150px">

# หลักการทำงาน
1.      เมื่อมีการกดปุ่ม switch การทำงาน
2.      ฟังก์ชั่นการ random ตัวเลขจะเริ่มทำการสุ่มตัวเลขขึ้นมาและจะเริ่มการทำงานทันที
3.      เมื่อมีการสุ่มตัวเลขทั้งหมดเสร็จ หลอดไฟ LED ทั้ง6ดวงจะขึ้นตามตัวเลขที่ฟังก์ชั่น random ได้ลูปขึ้นมา
4.      หลังจากนั้น 7-segment display จะขึ้นตามตัวเลขที่หลอดไฟ LED ที่ได้ปรากฎเมื่อสักครู่
<img src="https://github.com/MyNNeiei/AboutC_project/blob/main/Circurit.PNG">

โปรแกรมการทำงานของวงจร Smart Dice : https://www.tinkercad.com/things/0Q0A5c8MR0S-bodacious-luulia/editel?sharecode=c8WC7zmIZEIyshW-YH5nPVlcUAl67TDmga5AnHoQYaM

# Website Project
https://nickanyp.github.io/Project-Compro/

# YouTube สาธิตการทำงาน
https://www.youtube.com/watch?v=vNhkyRTJzG8

# Source Code
<img src="https://cdn.discordapp.com/attachments/963437675103289404/971074275949834280/1.PNG">
<img src="https://cdn.discordapp.com/attachments/963437675103289404/971074276218261554/2.PNG">
<img src="https://cdn.discordapp.com/attachments/963437675103289404/971074276503486484/3.PNG">
<img src="https://cdn.discordapp.com/attachments/963437675103289404/971074276964831282/4.PNG">
<img src="https://cdn.discordapp.com/attachments/963437675103289404/971074277170376734/5.PNG">

# Member
1.      นางสาวกุลนันท์ สุนันท์ 65070023
2.      นายณภัทร มากสมบูรณ์ 65070062
3.      นายณัฐวัตร จันโท 65070084
&emsp;&emsp;รายงานนี้เป็นส่วนหนึ่งของวิชา Physical Computing สาขาวิชาเทคโนโลยีสารสนเทศ ภาคเรียนที่ 1 ปีการศึกษา 2566 คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง
