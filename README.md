# Pull_Shark
~~~ Pull_Shark
# 프로젝트명

사용자가 선택한 조건을 바탕으로 결과를 생성하고, 직관적인 화면을 통해 확인할 수 있는 웹 애플리케이션입니다.

## 📌 프로젝트 소개

이 프로젝트는 프론트엔드와 백엔드를 분리하여 개발한 웹 서비스입니다.
사용자는 화면에서 원하는 옵션을 선택하고, 서버는 선택된 데이터를 기반으로 결과를 계산하여 응답합니다.

단순히 화면을 구성하는 것에 그치지 않고, API 연동, 데이터 검증, 예외 처리, 배포를 고려한 구조로 구현하는 것을 목표로 했습니다.

## 🛠 기술 스택

### Frontend

* React / Next.js
* TypeScript
* CSS Modules
* Axios 또는 Fetch API
* MSW

### Backend

* Java 17
* Spring Boot
* Spring Web
* Spring Data JPA
* MySQL
* Swagger

### Tools

* IntelliJ IDEA
* WebStorm
* Git / GitHub
* Docker

## ✨ 주요 기능

* 사용자 옵션 선택 기능
* 선택된 옵션 기반 결과 생성
* API 요청 및 응답 처리
* 로딩 화면 제공
* 결과 화면 제공
* 에러 발생 시 별도 에러 화면 제공
* 백엔드 API 문서화
* 서비스 로직 테스트

## 📁 프로젝트 구조

```bash
project
├── frontend
│   ├── app
│   ├── components
│   ├── api
│   └── styles
│
└── backend
    ├── controller
    ├── service
    ├── dto
    ├── entity
    ├── repository
    └── config
```

## 🚀 실행 방법

### Frontend 실행

```bash
cd frontend
npm install
npm run dev
```

### Backend 실행

```bash
cd backend
./gradlew bootRun
```

## 🔗 API 예시

### 옵션 목록 조회

```http
GET /api/options
```

### 결과 생성

```http
POST /api/result
```

요청 예시:

```json
{
  "selectedOptions": ["option1", "option2", "option3"]
}
```

응답 예시:

```json
{
  "result": "success",
  "message": "결과가 생성되었습니다."
}
```

## 🧪 테스트

백엔드의 주요 서비스 로직은 테스트 코드를 작성하여 검증했습니다.

테스트 항목은 다음과 같습니다.

* 선택 옵션 개수 검증
* 결과 생성 로직 검증
* 예외 상황 검증
* Controller API 응답 검증

## 💡 개발하면서 고민한 점

* 프론트엔드와 백엔드의 역할 분리
* API 요청 실패 시 사용자 경험 처리
* 모바일 화면에서도 자연스럽게 보이는 반응형 UI
* 서버 로직을 테스트하기 쉬운 구조로 분리
* 단순 구현이 아닌 유지보수 가능한 코드 구성

## 📚 배운 점

이번 프로젝트를 통해 화면 구현뿐만 아니라 백엔드 API 설계, 데이터 검증, 예외 처리, 테스트 코드 작성까지 전체적인 웹 서비스 흐름을 경험할 수 있었습니다.

또한 새로운 라이브러리와 도구를 두려워하지 않고 직접 적용해보며, 문제를 단계적으로 해결하는 개발 방식을 익힐 수 있었습니다.

## 📝 향후 개선 사항

* 사용자 경험을 위한 애니메이션 추가
* 배포 환경 최적화
* API 응답 구조 개선
* 테스트 코드 범위 확장
* 관리자 기능 추가

```
```
