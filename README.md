# ✨ 최신 영화 개봉 정보 및 리뷰 뉴스 모니터링

## 📌 프로젝트 소개
이 프로젝트는 네이버 뉴스 API를 활용하여 **최신 영화 개봉 정보 및 리뷰 뉴스**를 자동으로 수집하고 저장하는 프로그램입니다.
수집된 뉴스 제목과 관련 이미지는 파일로 저장되며, 이를 통해 최신 영화 트렌드를 쉽게 모니터링할 수 있습니다.

## 🚀 주요 기능
- 🎬 **최신 영화 개봉 정보 자동 수집**
- 📰 **영화 리뷰 뉴스 저장**
- 🖼️ **관련 이미지 다운로드**
- 📂 **파일로 뉴스 제목 저장**
- 🛠️ **로그를 통해 수집 과정 확인**

## 🔧 기술 스택
- **언어:** Java 11+
- **HTTP 통신:** `java.net.http.HttpClient`
- **파일 처리:** `java.io.FileWriter`
- **로깅:** `java.util.logging.Logger`
- **API:** 네이버 검색 API (뉴스, 이미지)

## 📂 프로젝트 구조
```bash
auto_monitoring/
├── src/
│   ├── App.java          # 메인 실행 파일
│   ├── Monitoring.java   # 뉴스 데이터 처리 클래스
│   ├── SortType.java     # 정렬 타입 enum
├── .env                  # API 키 설정 파일 (예: NAVER_CLIENT_ID, NAVER_CLIENT_SECRET)
├── README.md             # 프로젝트 설명
└── output/               # 저장된 뉴스 및 이미지 파일
```

## 🔑 API 키 설정
이 프로젝트를 실행하려면 **네이버 검색 API** 키가 필요합니다.
`.env` 파일을 생성하고 다음과 같이 설정하세요.

```bash
NAVER_CLIENT_ID=여기에_클라이언트_ID_입력
NAVER_CLIENT_SECRET=여기에_클라이언트_시크릿_입력
```

## 🏃‍♂️ 실행 방법
1. **프로젝트 클론 및 빌드**
   ```bash
   git clone https://github.com/soheeGit/auto_monitoring.git
   cd auto_monitoring
   ```
2. **환경 변수 설정** (API 키 입력)
3. **프로그램 실행**
   ```bash
   javac App.java
   java App
   ```

## 📌 사용 예시
- **최신 개봉 영화 소식 자동 저장**
- **영화 리뷰 및 평점 관련 뉴스 모니터링**
- **주요 영화 관련 이미지 다운로드 및 정리**
