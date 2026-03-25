# ToiletSystem
아두이노, 라즈베리파이, 모바일 앱을 연결하여  
환경 데이터를 수집하고 환풍기를 제어하는 IoT 시스템입니다.

<img width="398" height="575" alt="image" src="https://github.com/user-attachments/assets/a4865e5e-2fc3-4dbe-a251-80cf74eeac53" />


Firebase를 통한 데이터 받기 이후 처음 받은 값을 토대로 기준점을 잡아 초과시에 스마트폰 진동과 자동 환풍기 실행 구현,
일정 시간 지나도 초과 유지될시에 자동 물내림 구현
<img width="1278" height="637" alt="image" src="https://github.com/user-attachments/assets/06baed28-ac7c-445d-a296-3a0748d223dd" />

---

##  Data Flow

1. Arduino → 센서 데이터 수집  
2. Bluetooth → Raspberry Pi 전송  
3. Raspberry Pi → 데이터 처리 및 서버 역할  
4. Wi-Fi → Mobile App 통신  
5. App → 환풍기 제어 및 데이터 확인  

---

##  System Design

- Arduino → 센서 데이터 수집 전담  
- Raspberry Pi → 통신 및 처리 허브  
- Mobile App → 사용자 인터페이스  

- 역할 분리를 통해 시스템 확장성을 고려했습니다.

---

##  Communication

- Bluetooth (Arduino → Pi)
- Wi-Fi (Pi ↔ App)

---

##  Focus

이 프로젝트에서는 기능 구현보다  
**여러 장치 간 데이터 흐름과 통신 구조 설계**에 집중했습니다.

---

##  What I Learned

- IoT 시스템에서 데이터 흐름 설계가 핵심이라는 것을 배웠습니다.
- 서로 다른 통신 방식을 결합하는 구조를 구현했습니다.
- 장치 간 역할 분리가 시스템 확장성에 중요함을 이해했습니다.



라즈베리 파이 코드
<details>
  <summary>이미지 보기 </summary>
  <img src="https://github.com/user-attachments/assets/ce330a4b-3e4f-4127-bda1-221dd852d099"/>
  <img src="https://github.com/user-attachments/assets/f9ea96bc-e0e6-4b8f-a30a-1ebd25acb981"/>
  <img src="https://github.com/user-attachments/assets/962c5d06-31a6-4e71-970a-f96f7d2167b0"/>
  <img src="https://github.com/user-attachments/assets/4214a861-3c6b-45b6-b008-64fa47ee1cf2"/>
  <img src="https://github.com/user-attachments/assets/1d4c9028-a27d-4e97-affb-0622afd1a786"/>
</details>

