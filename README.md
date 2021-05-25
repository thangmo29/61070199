# ระบบตรวจจับถ้าเป็นนาฬิกาเเล้วไฟจะติด

 ![image](https://user-images.githubusercontent.com/41448294/119349907-ed8f3a80-bcc8-11eb-9c13-8c30400be314.png)

# ขั้นตอนการติดตั้ง
***# Install***
  - sudo apt-get update
  - sudo apt-get dist-upgrade
  - sudo apt-get install python-picamera
  - pip3 install opencv-python
  - pip install numpy
  - pip3 install tensorflow

***# ทำการ Enable Camera***
![Uploading image.png…]()

***# Download this repository and create virtual environment***
  - git clone https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi.git

***# Create Folder***
  - mv TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi tflite1
  - cd tflite1

***# Install and create the "tflite1-env" virtual environment***
  - sudo pip3 install virtualenv
  - python3 -m venv tflite1-env

***# เปิดการใช้งาน virtual environment***
  - source tflite1-env/bin/activate

***# Install TensorFlow Lite and OpenCV***
 - bash get_pi_requirements.sh
 
***# Set up TensorFlow Lite detection model***
 - wget https://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip 
 - unzip coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip -d Sample_TFLite_model
 
 ***# Run the TensorFlow Lite model***
  - python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model

# ขั้นตอนการใช้งาน
1. cd tflite1 เพื่อเข้าไปโฟลเดอร์ที่เก็บไฟล์
2. เปิด Virtual Environment โดยพิมพ์ source tflite1-env/bin/activate
3. จากนั้นทำการรันไฟล์ด้วยการพิมพ์ python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model

เว็บไซต์อ้างอิง : https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/blob/master/Raspberry_Pi_Guide.md
