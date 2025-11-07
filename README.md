<p align="center">
    <img src="https://github.com/user-attachments/assets/8040a8f4-e137-47ea-99e9-8aeaa64008ac" width="300" />
</p>

> 그로우잇은 음성 기반 AI와 대화하며 일기를 기록하고, 개인 맞춤형 마음챙김 챌린지를 제공해 정신 건강을 체계적으로 관리하는 앱입니다.

# ✨Project Information
> IT 연합 사이드 프로젝트 동아리 UMC-7th (GrowIt 프로젝트 Android 파트) 
> 
> 개발기간: 2025.12 ~


# Tech Stack과 Project Structure는 작업하면서 업데이트 예정

## 🚀 Tech Stack

### Framework & Library

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)
![XML](https://img.shields.io/badge/XML-555555?logo=w3c&logoColor=white)
![Jetpack_ViewBinding](https://img.shields.io/badge/Jetpack%20ViewBinding-34A853?logo=android&logoColor=white)
![Glide](https://img.shields.io/badge/Glide-0FAAFF?logo=android&logoColor=white)
![Retrofit2](https://img.shields.io/badge/Retrofit2-2C3E50)
![Gson](https://img.shields.io/badge/Gson-4285F4?logo=google&logoColor=white)
![Kotlin_Coroutines](https://img.shields.io/badge/Kotlin%20Coroutines-7F52FF?logo=kotlin&logoColor=white)
![MVVM](https://img.shields.io/badge/MVVM-6C63FF)

### Push & Messaging

![Firebase%20Cloud%20Messaging](https://img.shields.io/badge/Firebase%20Cloud%20Messaging-FFCA28?logo=firebase&logoColor=black)

## 📂 Project Structure

```text
.
├─ app/
│  ├─ build.gradle                  # 앱 모듈 빌드 스크립트
│  └─ src/
│     └─ main/                      # 실제 앱 코드
│        ├─ AndroidManifest.xml     # manifest
│        ├─ java/
│        │  └─ com/example/growitandroid/
│        │     ├─ application/                     # 앱 전역 설정/시작 지점
│        │     ├─ data/             # 데이터 계층 (Clean/Layered)
│        │     │  ├─ remote/        # 원격 데이터(API)
│        │     │     ├─ model/      # 요청/응답 DTO
│        │     │     ├─ service/    # 네트워크 호출 래핑(Service)
│        │     │     └─ repository/ # Repository (local/remote 조합)
│        │     ├─ ui/               # 프레젠테이션 계층
│        │     └─ utils/                   # 공통 유틸(비즈니스 무관한 순수 함수/헬퍼)
│        │
│        └─ res/                    # 리소스
│           ├─ drawable/            # 벡터/이미지 리소스
│           ├─ font/                # 폰트
│           ├─ layout/              # 화면 XML (Fragment/Activity/Item)
│           ├─ menu/                # 메뉴 XML
│           ├─ values/              # colors.xml, strings.xml, styles.xml 등
└─ README.md                        # 프로젝트 문서(구조/빌드/실행 방법)
```


## 🛠️ Branch Strategy

### 브랜치 유형

| 브랜치 유형 | 내용 |
| --- | --- |
| `main` | 완성된 버전의 코드를 저장하는 브랜치 |
| `dev` | 개발이 진행되는 동안 완성된 코드를 저장하는 브랜치 |
| `feat` | 작은 단위의 작업이 진행되는 브랜치 |
| `hotfix` | 긴급한 오류를 해결하는 브랜치 |

### 브랜치 명

- 유형/#이슈번호
    
    ex) feat/#30,  setting/#1
    

| 카테고리 | 내용 |
| --- | --- |
| `feat` | 구현 |
| `mod` | 수정 |
| `add` | 추가 |
| `del` | 삭제 |
| `fix` | 버그 수정 |
| `refactor` | 리팩토링 |

## 📔 Git Convention

### Git Flow

1. Issue 생성
2. Branch 생성
3. Add - Commit - Push - Pull Request(PR)
    1. Commit은 최대한 자주, 적은 양
    2. Commit시에 Issue를 연결
4. PR이 작성 후 충돌사항 없으면 merge하기
5. 새로운 작업을 시작할 때 dev에서 pull 받아오기

### Issue Convention

[카테고리] 제목 

ex) [INIT] 프로젝트 초기 세팅 

### Commit Convention

[커밋 카테고리/#이슈번호] 커밋 내용 (대문자)

ex) [FEAT/#30] 홈 뷰 구현, [ADD/#1] 폰트 파일 추가

| 커밋 카테고리 | 내용 |
| --- | --- |
| `feat` | 기능 (feature) |
| `fix` | 버그 수정 |
| `docs` | 문서 작업 (documentation) |
| `style` | 포맷팅, 세미콜론 누락 등, 코드 자체의 변경이 없는 경우 |
| `refactor` | 리팩토링 : 결과의 변경 없이 코드의 구조를 재조정 |
| `test` | 테스트 |
| `chore` | 변수명, 함수명 등 사소한 수정 *ex) .gitignore* |

### PR Convention

[카테고리/#이슈번호] 제목

ex) [FEAT/#6] 로그인 뷰 구현


## 📑 사용 예정 기술 스택 및 라이브러리

| 구분 | 기술 / 라이브러리 | 설명 |
| --- | --- | --- |
| 언어 | Kotlin | 안드로이드 앱 개발을 위한 주요 언어
| UI 구성 | XML / Jetpack ViewBinding | 뷰 레이아웃 구성 및 바인딩 처리
| 이미지 로딩 | Glide | 네트워크 또는 리소스에서 이미지 비동기 로딩 및 캐싱 
| 네트워크 통신 | Retrofit2 + Gson | REST API 요청 및 JSON 파싱
| 비동기 처리 | Kotlin Coroutines | 비동기 작업을 효율적으로 처리하기 위한 코루틴 사용
| 앱 아키텍처 | MVVM | Model-View-ViewModel 아키텍처 적용
| 푸시 알림 | FCM(Firebase Cloud Messaging) | 알림 메시지 수신 처리


## ⚙️Android Studio 환경 설정
버전 : Meerkat

targetSDK : 35

minSDK : 26

테스트 환경 : Emulator(Pixel 8a), Samsung Galaxy S22+
