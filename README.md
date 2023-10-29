# BEEP WITH ULTRASONIC SENSOR

# ที่มาของโครงงาน
&emsp;&emsp;ในปัจจุบันอินเทอร์เน็ตได้มีบทบาทในชีวิตประจำวันของพวกเราเป็นอย่างมาก ซึ่งได้ทำให้พวกเราได้นำความรู้เกี่ยวข้องกับ Arduino มาทำโครงงานเซ็นเซอร์รักษาความปลอดภัย เนื่องจากเซ็นเซอร์รักษาความปลอดภัยที่ทำจาก Arduino มีราคาที่ถูกกว่าและมีประสิทธิภาพที่ใกล้เคียงกับของตามท้องตลาดเพื่อใช้ทดแทนกันได้

# จุดประสงค์
- เพื่อให้ผู้ใช้สามารถใช้งานเซ็นเซอร์เพื่อรักษาความปลอดภัยภายในบ้านได้
- เพื่อเป็นรุ่นทดลองในการเอาไปพัฒนาต่อให้ดียิ่งขึ้นได้
- เพื่อให้ได้เซ็นเซอร์รักษาความปลอดภัยในราคาที่ประหยัด

# ประโยชน์
- ผู้ใช้ได้รับความปลอดภัย
- ผู้ใช้สามารถซื้อมาทำเองได้ง่ายและประหยัดกว่าไปซื้อแบบสำเร็จรูป
- ได้ฝึกฝนทักษะการทำ Arduino
- ได้ความรู้ในการต่อวงจรไปใช้ในชีวิตประจำวัน

# Poster
<img src="https://github.com/MyNNeiei/AboutC_project/blob/main/%E0%B9%82%E0%B8%9B%E0%B8%AA%E0%B9%80%E0%B8%95%E0%B8%AD%E0%B8%A3%E0%B9%8C.png" width="100%">

# อุปกรณ์
- Arduino UNO
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQsR8s4x-Aiywlqgw3OVy0u8jUW8uJ-V3mstw&usqp=CAU" width="150px">

- BreadBoard
<img src="https://inwfile.com/s-fp/ottf4f.jpg" width="150px">

- สายจัมพ์เปอร์
<img src="https://www.tido.tech/wp-content/uploads/2020/09/%E0%B8%9C%E0%B8%B9%E0%B9%89-%E0%B9%80%E0%B8%A1%E0%B8%B5%E0%B8%A2.jpg" width="150px">

- Ultrasonic Sensor
<img src="https://inwfile.com/s-dm/scscev.jpg" width="150px">

- Buzzer
<img src="https://static.robomart.com/image/cache/catalog/RM000338/piezo-buzzer-b-10n-piezo-electric-buzzers-rm0338-by-robomart-399-500x500.jpg.webp" width="150px">

# หลักการทำงาน
1.      ทำการเสียบตัวของ USB เข้ากับแหล่งกำเนิดไฟเช่น พาวเวอร์แบงค์
2.      ติดตั้งให้ตัวของ Ultrasonic sensor หาไปด้านนอกที่ต้องการให้มันตรวจจับสิ่งของที่เข้ามาใกล้
3.      เมื่อมีวัตถุหรือสิ่งของผ่านมาด้านหน้าของ Ultrasonic sensor ในระยะที่กำหนดตัว ลำโพงจะทำการส่งเสียงเตือน
<img src="https://github.com/MyNNeiei/AboutC_project/blob/main/Circurit.PNG">

โปรแกรมการทำงานของวงจร BEEP WITH ULTRASONIC SENSOR : https://www.tinkercad.com/things/gpmrNGYOjk8?sharecode=jUjotI3MGgs45FMWjk-l50TRAoaBrZhdh2c0xE6BBdk

# Website Project
https://mynneiei.github.io/AboutC_project/

# วิดีโอสาธิตการทำงาน
https://youtu.be/FyxdC8EgpBw?si=d3bWtFdo_XfDk0Or

# Source Code
    void setup()
    {
        Serial.begin(9600);
        pinMode(6, OUTPUT);
        pinMode(5, INPUT);
        pinMode(2, OUTPUT);
    }
    void loop()
    {
        long period, length;
        float new_delay;
        digitalWrite(6, LOW);
        delayMicroseconds(2);
        digitalWrite(6, HIGH);
        delayMicroseconds(10);
        digitalWrite(6, LOW);
        period = pulseIn(5, HIGH);
        length = (period / 2) / 29.1;
        if (length < 50)
        {
            if (length < 10)
            {
                new_delay = 50;
            }
            else
            {
                new_delay = (length * 3) + 30;
            }
            digitalWrite(2, HIGH);
            delay(new_delay);
            digitalWrite(2, LOW);
        }
        else
        {
            digitalWrite(2, LOW);
        }
        Serial.print(length);
        Serial.println(" cm");
        delay(200);
    }

# สมาชิกกลุ่ม
1.      นางสาวกุลนันท์ สุนันท์ 65070023
2.      นายณภัทร มากสมบูรณ์ 65070062
3.      นายณัฐวัตร จันโท 65070084
