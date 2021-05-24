# ระบบตรวจจับโทรศัพท์เเล้วไฟติด
- ทำระบบตรวจจับวัตถุเเล้วเเสดงสีออกทางหลอดไฟ
- ใช้ Opencv & TensorFlow
   ![image](https://user-images.githubusercontent.com/41448294/119343383-8ff6f000-bcc0-11eb-94e7-89cf51fa9fe6.png)
  # ขั้นตอนการติดตั้ง
# Install
  - sudo apt-get update
  - sudo apt-get dist-upgrade
  - sudo apt-get install python-picamera
  - pip3 install opencv-python
  - pip install numpy

# Download this repository and create virtual environment
  - git clone https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi.git

# Create Folder
  - mv TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi tflite1
  - cd tflite1

# Install and create the "tflite1-env" virtual environment
  - sudo pip3 install virtualenv
  - python3 -m venv tflite1-env

# เปิดการใช้งาน virtual environment
  - source tflite1-env/bin/activate


       # ขั้นตอนการใช้งาน
1. cd tflite1 เพื่อเข้าไปโฟลเดอร์ที่เก็บไฟล์
2. เปิด Virtual Environment โดยพิมพ์ source tflite1-env/bin/activate
3. จากนั้นทำการรันไฟล์ด้วยการพิมพ์ python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model

เว็บไซต์อ้างอิง : https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/blob/master/Raspberry_Pi_Guide.md
