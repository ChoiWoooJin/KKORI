# 🐶 강아지 산책대행 프로젝트 KKORI 🐶
<div align="center">
  <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/7076d691-7933-4389-a06e-5de73416dcfd" width="200" hight="200">
</div>

# 프로젝트 소개 😊

* 프로젝트명: 너와 나의 연결 KKORI
* 주요 기능
  - BLE,UWB 기기를 통한 반려견 관리
  - 반려견 위치 추적 및 산책현황
  - 게시판, 로그인, 지도
  - real time 채팅
  - QR 인증을 통한 산책대행 관리
* 주요 기술
  - EC2, S3, firebase

  - ReactNative.js, Node.js, Expo, android

  - Springboot, Spring Security, JPA, QueryDSL, JWT Authentication, OAuth, REST API

* 참조 리소스
  * 구글맵
  * 카카오 주소 api : 주소를 지번으로 변환후 지번을 추출하여 위도경도로 변환
  * gifted-chat : 디자인 전반적 사용
  * firebase : realtime DB에 채팅 저장, 산책현황좌표 기록 후 산책 루트 드로잉
  * lottiefiles: 메인 페이지 진입 애니메이션에 활용
* 배포 환경
  -https://drive.google.com/file/d/1o74JpKF7mp-bgxnmIbbMmZ_E3pIn_8e4/view?usp=sharing



# KKORI 기획:satellite:

1인가구 증가에 따라 혼자있는 반려견이 많아졌다. 하지만 야근이라도 하는날 반려견은 산책이 힘들다는걸 인지하였다.<br>
하지만 비싼돈을 주고 전문인력이나 경험부족의 사람에게 맡기기에는 선뜻 반갑지않다<br>
이러한 문제를 해결하고자 **하이퍼 로컬기반 강아지산책대행**의 필요성을 인지하게 되었습니다.

# KKORI 소개📄
* KKORI는 블루투스기기를 통하여 산책현황 및 반려견 관리를 할수있습니다.:astonished:
* 게시글 등록후 **채팅**을통해, 다른 유저와 **예약**이 가능합니다.:film_frames:
* **위치기반**내 주변 게시글을 볼수있습니다. :100:
* 사용자 간의 자유로운 예약을 활성화 하고 기기를 통한 반려견의 안정성을 향상시켰습니다	:clap:

# 기능 소개💡
* KKORI 주요 기능은 다음과 같습니다

## 메인 및 게시판 🟡

| 앱로딩-메인 | 게시판 |
|:---:|:---:|
| <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/fe8923f2-395a-4c69-9ec3-820558f541dd" width="300"> | <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/6626018b-0f9b-40ad-9638-82ca37818ebf" width="300"> |
| 앱 시작 화면입니다! | 게시판 화면입니다! |

- 메인화면에는 지도게시판, 산책현황, QR인식, 산책왕, 분실견이 있습니다.
- 하단네비에는 메인, 게시판(게시글로 보는), 채팅, 마이페이지가 있습니다.
- 메인페이지 화면설계는 스텍식으로 설계하였습니다.
- 하단네비바는 자주 사용하는 컴포넌트로 설계하였습니다.

## 채팅 및 지도 🗨

| 채팅 | 지도 및 클러스팅 |
|:---:|:---:|
| <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/d1f6e234-17e7-422e-815a-462d4f0f1d31" width="300"> | <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/c7e97ca3-c14b-44fa-af7d-8c265898874a" width="300"> |
| 게시판에서 견주에게 채팅을 보낼 수 있습니다! | 내 위치 기반 게시글을 볼 수 있습니다! |

- 게시글작성은 제목, 가격, 위치, 내용, 나의 반려견을 선택 및 작성하여야 합니다.
- 위치는 위도경도로 변경되어 반환되며, 정확환 위치를 마킹하지 않습니다.
- 반려견을 여러마리를 한번에 산책등록할수있습니다.

## 관리 🕔

| 반려견 관리 | 산책 현황 |
|:---:|:---:|
| <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/79ab14af-9a46-4cde-a296-16a78a5d666e" width="300"> | <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/11fce1e6-b512-4adb-bfe3-c1d96d2c0cce" width="260"> |
| 나의 반려견을 관리할수있습니다! | 실시간 산책현황이 드로잉됩니다! |

- 기기당 최대 5마리까지 반려견을 등록할수있습니다.
- 예약을 진행한후 QR을 찍으면, 예약된 게시물이 표시된후 산책이 시작됩니다.
- 실시간으로 거리가 표시되며, 기기와 QR인증한 휴대폰이 멀어지면 알림이 갑니다.


# 사용Tool
![kkori_tool](https://github.com/non-inss/KKORI-SSAFY/assets/122503960/a8189352-66af-4b74-868e-78ce06912d0c)

# API 연동 규격서 

[API 연동규격서 2975d5ee4025451b86d5de19703ef893.pdf](https://github.com/non-inss/KKORI-SSAFY/files/13446920/API.2975d5ee4025451b86d5de19703ef893.pdf)

# 시스템 구조도🏗️

![아키텍처](https://github.com/non-inss/KKORI-SSAFY/assets/122503960/bd179587-75fb-415e-9d14-6191188051d7)




