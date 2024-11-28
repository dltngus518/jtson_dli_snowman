# jtson_dli_snowman


# 목차

# 1.SD 카드 준비

# 2.JetPack 설치

# 3.Jetson Nano 설정

# 4.Ubuntu 설치

# 5.한글 환경 설정

# 6.카메라 설정

# 7.Docker 및 Jupyter 설치

# 8.Classification 프로젝트





## 1.SD 카드 준비
   
-sd카드 포멧팅하고 다운로드받는다.

![image](https://github.com/user-attachments/assets/cfe36cec-fc62-472c-86d0-76e133957d94)

-balenaEtcher 다운로드, jetpack 4.6다운로드
![image](https://github.com/user-attachments/assets/c10ca178-e5d6-458e-934a-f8a7e7473b92)


-microSD카드에 jetson파일 다운로드(이미지를 굽는다,burning한다)
   ![image](https://github.com/user-attachments/assets/2caa9b74-cfa8-40c0-9560-afb9b1d52c6c)
gui=graphic user interface


## 2. JetPack 설치
   
   -SD 카드를 Jetson Nano에 삽입
   
## 3.Jetson Nano 설정

![image](https://github.com/user-attachments/assets/f2785571-9f20-4fef-8aa2-fe6cb6b87a41)

-각 단자 연결

-싱글보드 컴퓨터 생성
    -주의사항 : sd카드 넣고 뺄때 가볍게 눌러준다


## 4.우분투 설치

-부팅 후 우분투 설치
-기본 설정 완료 : 네트워크 연결, 계정생성 등
-필요한 라이브러리와 패키지를 업데이트

![image](https://github.com/user-attachments/assets/eb96c24c-2617-461b-875f-5276ef7d2f62)

![image](https://github.com/user-attachments/assets/05823b33-17b3-408b-a36b-2c78dccb69af)

![image](https://github.com/user-attachments/assets/c7c59c3c-d58e-4bf4-89f0-03de8d9b6176)

![image](https://github.com/user-attachments/assets/e6e9dcb2-8119-4704-8f12-5af727798b13)

![image](https://github.com/user-attachments/assets/7b028654-755a-4152-96ab-ddeca7b28700)

![image](https://github.com/user-attachments/assets/b1e8b788-b561-4f2c-a474-f76fc3982c74)



## 5. 한글설치

-sudo apt-get update 

![image](https://github.com/user-attachments/assets/8d7b898d-de4f-4d52-bc45-1411b1072ec6)

- sudo apt-get install fcitx-hangul
  
![image](https://github.com/user-attachments/assets/5e054002-b8af-418f-931e-7f383ea6692f)

-configure

![image](https://github.com/user-attachments/assets/5e7d671b-531a-41ab-920a-f62e9858e62b)

-hangul찾아서 체크

![image](https://github.com/user-attachments/assets/020efd0f-bb39-49d6-b066-f568188864e5)

-시스템 재부팅 후 한글 입력 확인인


## 6. 카메라 설치 및 연결
    1) 카메라를 젯슨에 연결
    2) dli@dli-desktop:~$  ls /dev/vi* -작성하여 카메라 인식하는지 확인
![image](https://github.com/user-attachments/assets/2cb047f0-6156-4740-b5f9-b61dc1d2f8ce)

    3) dli@dli-desktop:~$ git clone https://github.com/jetsonhacks/USB-Camera.git - 카메라 불러오는 명령어
![image](https://github.com/user-attachments/assets/d04d56e6-d2e4-474a-852b-2f4d02d1dc10)


    4) dli@dli-desktop:~/USB-Camera$ python3 usb-camera-gst.py 실행시 카메라
  
   
   ![image](https://github.com/user-attachments/assets/da051c1f-9562-436a-9342-13f9fff575ae)


    5) dli@dli-desktop:~/USB-Camera$  python3 face-detect-usb.py 실행시 카메라
  
       
   ![image](https://github.com/user-attachments/assets/f0fda729-01f3-4a76-b302-64d543ddf060)


    6) csi 카메라 - 로봇에 달려있는 카메라
  
    
    7) dli@dli-desktop-/USB-Camera$ ls는하위폴더






## 7.Docker 및 jupyter 설치

-docker설치

![image](https://github.com/user-attachments/assets/8c825cd9-659b-4804-acca-102fba627b01)


-swap과정 
 -시스템 GPU모드로 설정


-주피터 실행

![image](https://github.com/user-attachments/assets/789f712c-d143-4ba6-a1db-60a06f65759a)


## 8.classification

-데이터 준비

![image](https://github.com/user-attachments/assets/13dcb171-b6a7-409b-bc7c-f2e4660a373d)

![image](https://github.com/user-attachments/assets/62e49273-efde-4dbb-be0f-32ed34dbed30)


-데이터 기반 train

![image](https://github.com/user-attachments/assets/6a3456ed-7f80-4d5d-87de-b1df35ab6a23)

-결과 확인 및 저장   


