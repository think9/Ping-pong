# QR Code 인식을 이용한 온라인 탁구 게임

## Ping-pong online game with QR-code

### 개요
* Tkinter 기반 탁구 게임
* 소켓 통신을 이용하여 다른 사람과 온라인 게임 진행
* pyzbar를 이용한 QR Code 인식
* openCV를 이용한 영상처리<br>

### 사용방법
* 두 사람이 함께 진행
* Player1 : server.py를 실행 후 pong(client-host).py를 실행
* Player2 : ip주소를 설정 후 pong(client).py<br>

### 개발 issue
* Socket 통신 속도 일치
  * 게임 진행 시 네트워크 지연으로 공 위치 불일치 현상 발생
  * host player를 지정하여 공의 위치를 상대에게 전송하여 해결
* QR Code 인식률 개선
  * openCV를 이용하여 색상 영역 검출 및 이진화 수행
  * 전처리를 통한 QR Code 인식률 상승

![개발 목표](https://user-images.githubusercontent.com/50393277/65743215-9e2ceb80-e12e-11e9-989d-9114edfae3cd.png)

![사용기술](https://user-images.githubusercontent.com/50393277/65743258-c87ea900-e12e-11e9-83f1-a0087240a148.png)

![프로그램 구조](https://user-images.githubusercontent.com/50393277/65743290-e21ff080-e12e-11e9-8db4-1ff8bc3f92b5.png)

![프로그램 수행 과정](https://user-images.githubusercontent.com/50393277/65743312-fb28a180-e12e-11e9-930a-c0232c51214a.png)

![통신 과정](https://user-images.githubusercontent.com/50393277/65743322-067bcd00-e12f-11e9-9e8e-9efc71811109.png)

![QR Code 검출](https://user-images.githubusercontent.com/50393277/65743331-0f6c9e80-e12f-11e9-946d-b39736191a4c.png)

![게임 화면](https://user-images.githubusercontent.com/50393277/65743337-185d7000-e12f-11e9-8ea6-555293ef0d54.png)
