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


