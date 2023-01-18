# SPCN-NMS
# ขั้นตอนการติดตั้ง Obsevium
![image](https://user-images.githubusercontent.com/119155285/210497288-4df9f0f4-938b-4dae-b0d4-69c5c070b798.png)
ในขั้นตอนแรก เราใช้โค้ดตัวนี้เพื่อ Set Time
### CODE Set Time
            timedatectl set-timezone Asia/Bangkok

ขั้นตอนต่อไป เป็นการ update upgrade โดยใช้โค้ดนี้
### CODE update upgrade
           apt update; apt upgrade -y
           
ขั้นตอนที่ 3 เป็นการติดตั้ง Obsevium ลงใน Ubuntu 20.04 โดยใช้โค้ดนี้ 
### CODE ติดตั้ง
          wget http://www.observium.org/observium_installscript.sh
          chmod +x observium_installscript.sh
          ./observium_installscript.sh
        
![image](https://user-images.githubusercontent.com/119155285/210498861-de237099-84a0-4a5d-b632-ce079294aad0.png)

จากรูป แก้ไข add-apt-repository: คําสั่งไม่พบข้อผิดพลาด
  ![image](https://user-images.githubusercontent.com/119155285/210499130-0e172638-3a8a-471e-a744-1bda597af26a.png)

วิธีแก่ไขข้อผิดพลาดก็คือ การใช้ sudo apt-get install software-properties-common
### CODE  แก้ข้อผิดพลาด
          sudo apt-get install software-properties-common -y
          
จากนั้นแก้ข้อผิดพลาดเรียบร้อยแล้ว เราก็กลับมาทำขั้นตอนที่ 3 ใหม่ อีกครั้งโดยใช้โค้ดเดิม

ขั้นตอนที่ 4 เมื่อเราติดตั้ง Obsevium เรียบร้อยแล้ว มันจะขั้นให้เราเลือกการติดตั้ง เราเลือกเป็น Choose : 1 แล้วกด Enter เพื่อเป็น install 
![image](https://user-images.githubusercontent.com/119155285/210499764-91d18a5b-3fc6-4be6-872b-d891cb8cd3b8.png)

ขั้นตอนที่ 5 เป็นการเลือก Y/N ดังรูป เราต้องเลือก Y ในการติดตั้ง
![image](https://user-images.githubusercontent.com/119155285/210500031-463189ce-5cc8-4d03-88e9-056896ee80cb.png)
![image](https://user-images.githubusercontent.com/119155285/210500064-29a78df5-526c-45c2-be8c-6b22f910d6e2.png)

ขั้นตอนที่ 6 เป็นการตั้ง Password ในการเข้าหน้า Wed Obsevium โดยเราจะใช้ admin ในการเข้าใช้ ในโปรแกรม จะให้เราใส่ Password 3 ครั้ง
![image](https://user-images.githubusercontent.com/119155285/210500690-dff218a5-b6f6-40c1-a654-a4bdcdfc4907.png)

ขั้นตอนที่ 7 เป็นการตั้ง Username ใน Obsevium
![image](https://user-images.githubusercontent.com/119155285/210505941-39615174-020c-4937-b978-99fdbb3fe9bc.png)

ขั้นตอนที 8 ดังรูป เลือก Y เพื่อทำการติดตั้งต่อ
![image](https://user-images.githubusercontent.com/119155285/210503389-8c5463ef-2ffc-4fda-aa19-599c63c24e0d.png)

ขั้นตอนที่ 9 เป็นการ install UNIX agent ให้ทำการเลือก Y เพื่อติดตั้งใช้งานควบคู่กัน
![image](https://user-images.githubusercontent.com/119155285/210503716-30cd4f0e-d762-4877-8fdf-a44710ee8977.png)

# ขั้นตอนการใช้งาน (SPCN-NMS)

ขั้นตอนที่ 1
 
- เข้า Local Host กับตัว Sever 

![image](https://user-images.githubusercontent.com/117635686/210507928-41fc3f3a-35a5-43e7-9b21-079cd419e863.png)

- ล็อคอินเข้ามาแล้วก็เจอกับหน้าดังรูป

![image](https://user-images.githubusercontent.com/117635686/210508426-e99621b6-9c61-457d-acb5-a428c9a86c82.png)

- แล้วกดตรงแถบเครื่องมือข้างบนแล้วกดเลือก Add Device

![image](https://user-images.githubusercontent.com/117635686/210508646-14af7521-8bc7-4178-b625-3720085bb463.png)

- ต่อมา ให้กดเข้าหน้า Basic Configuration

![image](https://user-images.githubusercontent.com/117635686/210508835-4a5cea6f-70bc-45ac-8cec-a729fed27930.png)

![image](https://user-images.githubusercontent.com/117635686/210509070-3d1be511-615b-43dd-8ffa-6d0ec4d8aa69.png)
# วิธีการ Add device

- ให้นำ IP ที่อาจารย์ให้ลงไปเติม หลังจากนั้น กด Add device

![image](https://user-images.githubusercontent.com/117635686/210510698-7ef57202-1af9-4b51-ac2a-c5c8425c1f5f.png)

![image](https://user-images.githubusercontent.com/117635686/210509352-650adbf0-f093-46f5-9a69-afb2e6f61b5b.png)

- หลังจากกด Add Deive แล้ว จะมีการแจ้ง IP ขึ้นมาดังรูป

![image](https://user-images.githubusercontent.com/117635686/210509660-2eb636d3-6413-4001-ab0e-24a5ba4e69dd.png)

- คลิกเพื่อเข้าไปดูข้อมูลดังรูป

![image](https://user-images.githubusercontent.com/117635686/210509885-a554c116-a047-4f17-a86b-577347304cd6.png)

- หลังจากนั้นรอภายใน 1 วัน เพื่อรอให้มันตรวจสอบเพราะว่ามันยังไม่สามารถระบุได้ภายในทันที

![image](https://user-images.githubusercontent.com/117635686/210510186-b2e6c0e1-8da1-44c5-b49f-6e372c28d0d9.png)

- หลังจากครบ 1 วันจะได้ตามดังรูป

![image](https://user-images.githubusercontent.com/117635686/210831155-fe086e22-ff10-48b7-9a4a-63564325947c.png)

# การอ่านผลของเครื่องมือ

พอเข้ามาในเครื่องที่เราแอดไปแล้วในส่วนของ Overview ก็สามารถดูค่าต่างๆได้ ดังรูปได้แก่ Ports,Eventlog,Processors,Memory,Storage

![image](https://user-images.githubusercontent.com/117635686/210832336-4e51b4ae-28f8-4dc7-9149-54a9ee42dd31.png)

  - Ports

สามารถบอกจำนวนตัวอุปกรณ์และชื่อของ Ports ที่ทำการต่อเข้ามา  
  
  - Eventlog

สามารถดูประวัติรายงานเหตุการณ์ที่เกิดขึ้นได้

  - Processors

สามารถดูการทำงานของ Processors ได้
 
  - Memory

สามารถดูความจำในส่วนของ RAM ได้

  - Storage

สามารถบอกพื้นที่การเก็บข้อมูลได้ 

### เสริมรายละเอียด ในส่วน Health
### Processer
* สามารถเลือกดูกราฟแบบรายนาที รายวัน รายสัปดาห์ หรือ รายปี
   * วิธีอ่าน Graph
     * แกน X คือค่าเวลาของ Graph
     * แกน Y คือค่า Processor ขณะที่ทำงานอยู่
* สามารถบอกค่าเฉลี่ย ของ Processer ได้ 

![image](https://user-images.githubusercontent.com/119155285/211134261-0bbb65af-f49b-488e-a060-51ca33b11ce9.png)

### Memory
- สามารถเลือกดูกราฟแบบรายนาที รายวัน รายสัปดาห์ หรือ รายปี
   * วิธีอ่าน Graph
     * แกน X คือค่าเวลาของ Graph
     * แกน Y คือค่า Memory ที่ใช้ตามเส้นสี
- สามารถบอกความจำในส่วนต่างๆ ของตัว Device ได้ 

![image](https://user-images.githubusercontent.com/119155285/211134469-a652e9d7-8773-43db-b0e1-e7409eb5cc7e.png)

### Storage
- สามารถเลือกดูกราฟแบบรายนาที รายวัน รายสัปดาห์ หรือ รายปี
   * วิธีอ่าน Graph
     * แกน X คือค่าเวลาของ Graph
     * แกน Y คือค่าพื้นที่เก็บข้อมูลบอกเป็นเปอร์เซ็น 
- สามารถบอกความจำในส่วนต่างๆ ของตัว Device ได้ 
  

![image](https://user-images.githubusercontent.com/119155285/211134574-fa2284b3-2c3d-4973-b49d-1e28a5edac55.png)

### Disk I/O
- สามารถเลือกดูกราฟแบบรายนาที รายวัน รายสัปดาห์ หรือ รายปี
   * วิธีอ่าน Graph
     * แกน X คือค่าเวลาของ Graph
     * แกน Y คือค่าปริมาณข้อมูลเข้าออก 
- สามารถบอกาอัตราการเข้า-ออกของข้อมูลได้ 

![image](https://user-images.githubusercontent.com/119155285/211134615-1cf2c681-fecc-48fb-88b6-671521490a34.png)

# สมาชิก
- https://github.com/teerasut01
- https://github.com/Hgot7
- https://github.com/Ruangrit-01
- https://github.com/Jirawat156




