# 차량 전장시스템 이해(240605~240610)
## 자동차 개요
### 구동 방식
  - FF: front 엔진 Front 구동
  - RR: Rear 엔진 Rear 구동
  - FR: Front 엔진 Rear 구동
  - 4WD: 사륜구동
    
### 내연차의 기본 구조
- 기관: 동력 발생 잔치(엔진,연료, 흡기, 배기)
- 섀시: 동력전달 장치(엔진제외한 클러치, 변속기, 현가, 조향, 제동)
- 전장: 전기장치(램프, 안전벨트, 실내등, 편의장치)

## 섀시
![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/dc0df85f-245d-41ee-a53d-529c9a7e9503)
- 조향장치: 방향제어(스티어링 휠)
- 현가장치
  - 진동/요철에 이한 차체의 움직임 상쇄
  - 원심력에 의한 차체 자세 제어(Shock absorber)
- 제동장치
  - 지면과의 마찰력  
  - 앞:뒤=80:20
  - 마우스 실린더: 압력을 가해줌
    

### 클러치: 기관과 수동변속기 사이에 부착, 동력 전달/차단
  - 플라이 휠: 텐션의 관성, 크랭킹(크랭킹 축을 이용하여 기동전동기 돌림)
   ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/b026897a-4a72-4465-a591-31dd8c39076b)

#### 자동 변속기
- 유체 클러치: 원심력에 의해 상대편 낱게 차 회전(기체)
- 토크 컨버터: 주행저항에 따라  구동력 변환(오일)
  - 속도 빠르면 오일 압력 빨라서 빨리 돌아감
  <img src="https://github.com/JiYoon402/IVS_notes/assets/90745522/75347dc0-81a6-49d2-ae41-3cfea7208527" width="500">
   <br/>    
- 전자제어 자동 변속기: 전자제어 장치와 연계하여 제어(TCU: Transmission Control Unit)=>신호 중요!)
  ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/9e902b08-3427-4c92-8672-0e66884c9750)
  - 스로틀 포지션 센서: 스로틀 밸브의 위치 개방 각도를 측정, 연료량을 조절하는 역
  - 펄스 제너레이터: 펄스로 자동 변속기 제어(pwn 듀티로 제어), 오일의 압력 이dyd
  - 점화 코일: 가솔린 차에서 연료 점화
  - 인히비터 스위치: 변속 단어 결정
  - 킥다운 서보, 아이들, 오버드라이브 스위치: 변속이 이루어져서 주행 할 때 스위치 작동, 주행시 변속기 작동 모니터링
  - 유온 센서: 오일로 작동하는 자동변속기의 오일 온도 제어
  - 차속 센서: 변속기에 붙어서 차의 속도 측정
  - 휠 스피드 센서: 바퀴의 회전 속도 측정
- 유성기어 장치: 링기어, 선기어, 유성기어, 캐리어로 구성
  - 더블클러치 기어 바꿀 때 미리 예측
  - 기어의 조합에 따라 출력이 달라짐
 <img src="https://github.com/JiYoon402/IVS_notes/assets/90745522/2f0e43f9-75c0-43ab-837e-ecb29634c7e5" width="400">
<img src="https://github.com/JiYoon402/IVS_notes/assets/90745522/ce009208-ffed-46bb-9c9c-4ec5caa0caf6" width="400">

### 현가 장치
#### 전자제어 현가장치의 제어기능
- 프리뷰 제어
- 스카이훅 제어
- ECS(Electronc Control Suspension System)
  ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/740fdce0-b13f-4bad-9b5c-9b6740139d15)
  - TPS:trutle position sensor
  - 차속 센서: Hall sensor
   <img src="https://github.com/JiYoon402/IVS_notes/assets/90745522/89515399-a559-4103-b3fa-32de1f414823" width="300">
  - 중력 가속도 센서: 에어백 작동 위해  

### 조향장치
#### 조향기구
- 동력 조향 장치: 피스톤 이용 유압식
- 전자제어 조향 장치: 배터리 전원 이용
  ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/961ab7af-37f2-426a-a1aa-6f6c599ff85c)

### 제동장치
- 전자제동력 분배장치
- ABS
- 통합제어 TCS
- CAN통신

<br/>

## 기관
### 기관의 4가지 과정
- 흡입
- 압축 ->온도 상승
- 폭발
- 동력 발생

### 기관의 주요 장치
- 캠축, 크랭크축의 타이밍이 맞아야지 작동이 된다
- WTS: 냉각
  ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/e6f1bcba-ddb5-4a07-a746-81f2df5cf249)
- 크랭크각 센서,캠축 포지션 센서: 홀센서
- 슬틀 포지션 센서
- 



## 전기
### 시동 장치
#### 기동 전동기
- 구성: 전동기, 솔레노이드, 오버로닝 클러치
![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/9e84cd6c-c07e-43b7-a46f-ceee1ae6f6d5)

### 점화 장치
#### HEI(High Energy Ingnotion): 고강력 점화 방식
- 코일 이용하여 점화플러그에 불꽃 방전(변압기 원리)
#### DLI
- 접점식 점화장치, 트랜지스터식(npn) 점화 장치
-  점화코일에서 점화플러그로 직접 배전

### 충전 장치
#### 충전 장치의 개요
- 교류 발전기: 정류용 Si다이오드에 의해 직류 출력 얻음
- 교류 발전기 조정기: 발생 전압 일정하게

### 공조 시스템
#### 냉방 장치 작동 원리
- 사이클: 증발-> 압축-> 응축-> 팽창 (순환반복)
![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/f998fc5a-a60d-4446-bfb8-f708ffd8dfcb)
- FATC(Full auto air con) 이용하여 제어
  

### 등화 장치
- BCM(Body Control Module) 이용하여 제어
![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/d845675a-400a-48b4-8ede-d3134aee3b1b)
#### 오토 라이트 장치
![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/f14baef3-eb91-476d-92d2-414c3809c488)

#### 스마트 전조등
- AFLS(적응형 전조등 시스템): 조향각 센서 이용
- SHBA(Smart high beam assist): 이미지 센서 이용

### 안전 장치
- 방향 지시등
- 제동등(stop lamp)
- 후진등(back-up lamp): 변속기에 설치(통신XXXX)
- 윈드 실드이퍼(wind shield wiper): 레인 센서(포토다이오드 이용)
- 전자제어 시간경보 장치(ETACS ; electronic, time, alarm, control, system): 각 컴퓨터로부터 정보 받아 알림/경보
  ![image](https://github.com/JiYoon402/IVS_notes/assets/90745522/33665185-33a6-4401-bfec-f4e93ac30f76)

  








